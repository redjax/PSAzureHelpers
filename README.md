# Powershell Azure Helpers Module

This module adds some helper functions to your Powershell `$PROFILE` for interacting with Azure.

## Setup

- Run this command to get a list of all the locations Powershell loads modules from: `$env:PSModulePath -Split ';'`
  - This will show you a list of paths, like `C:\Users\<your-username>\Documents\PowerShell\Modules` and `C:\Program Files\Powershell\Modules` or `C:\Program Files\Powershell\Modules` (for Powershell 7 modules).
- Copy the [`AzureHelpers` directory](./AzureHelpers/) to one of these locations.
  - Put it in your `Documents\PowerShell\Modules` path to load it for your profile only.
  - Place it in one of the `C:\Program Files` paths to load the module globally (i.e. including elevated sessions).
- Start a new Powershell session and run `Get-Module`
  - Look for `AzureHelpers` in the list. If you see it, it's installed!

## Usage

- To see a list of all the functions available from the `AzureHelpers` module, run: `Get-Command -Module AzureHelpers`
- To see the help menu for one of the functions, run `Get-Help <functionName>`, i.e. `Get-Help Search-KVSecret`
