# Teams-Transcript-Summariser-Open-AI
This is a repo for a Power Automate cloud flow solution that allows the user to summarise Teams transcripts using GPT4.

See here for more details - https://www.jondoesflow.com/post/teams-transcript-summariser-with-gpt4-in-power-automate

Please use the latest version. (1_0_0_3)

# Installation instructions

1. Download the latest version from the repo.
2. Go to https://make.powerapps.com
3. Select the right environment you want to import the solution into
4. Click Import Solution on the ribbon
5. Browse to the solution zip file
6. Click Next
7. Click Next again
8. Next you need to make sure you have an Open AI API key, you can get one from https://platform.openai.com
9. Then you need to go to https://portal.azure.com and click on App Registrations, give it a name and click register.
10. Take a copy of the Directory (tenant ) ID
11. Take a copy of the Application (client) ID
12. Click on API permissions and give all of these permissions to the App Registration:
![image](https://github.com/user-attachments/assets/73ecfc53-cc4d-42e3-bfe9-6cf38fab944f)
13. Click Grant Admin permission for <tenancy>
14. Click on Certificates and Secrets
15. Click New client secret
16. Make a copy of the value
17. Go back to the solution import, paste this in the **TS Graph Client Secret** field
18. Paste the Tenant ID (from step 10) in the **TS Graph Tenant ID** field
19. Paste the client ID (from step 11) in the **TS Graph Client ID** field

Next steps are optional:

21. Go to https://dev.azure.com (you will be promoted to sign in, and probably taken back to the Azure Portal)
22. Click on Azure DevOps Organisations
23. In the top right hand corner click the person cog icon:

![image](https://github.com/user-attachments/assets/49bb885d-ff9e-44d2-94ae-5c6c4b16c688)

24. Click Personal Access Token
25.Click New Token

![image](https://github.com/user-attachments/assets/e6627967-8ba4-4630-b6db-93d270b7d8b7)

27. Complete as per the screenshot
28. Click Create
29. Copy the Personal Access Token (PAT Token)
30. Click Close
31. Paste this in the **TS ADO PAT Key** field back on the solution import page
32. Click Import
