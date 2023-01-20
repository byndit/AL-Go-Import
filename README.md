# Import Template

This repo allows you to import repos based on old HelloWorld repository to AL-Go

1. Click "Use this template" > "Create a new repository"
2. Enter a name, choose the organisation and visibility and click "Create repository from template"
3. Make sure you have a organisation secret GHTOKENWORKFLOW setup like mentioned in the [Update Al-Go System Files Scenario](https://github.com/microsoft/AL-Go/blob/main/Scenarios/UpdateAlGoSystemFiles.md)
4. Note the clone URL of the repository you want to import.
   - Make sure to include the Personal Access Token in the URL if authentication is needed. (The PAT only need read access!)
     - [Github](https://docs.github.com/de/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
       - https://<PAT\>@github.com/...
     - [Azure DevOps](https://learn.microsoft.com/en-us/azure/devops/organizations/accounts/use-personal-access-tokens-to-authenticate?view=azure-devops&tabs=Windows)
       - https://<PAT\>@dev.azure.com/...
5. Once your repository is created, navigate to Action and run the "Import Repository" Action.
6. Enter the following inputs:

   - Import from URL: The clone URL of your existing repository
   - Template URL (@notation for branch selection is currently not supporteds):
     - https://github.com/microsoft/AL-Go-AppSource
     - https://github.com/microsoft/AL-Go-PTE

7. After the action has finished you will need to add your app folders to the corresponding settings and add other wanted settings. Check the [AL-Go Readme](https://github.com/microsoft/AL-Go/#readme) for additional information
