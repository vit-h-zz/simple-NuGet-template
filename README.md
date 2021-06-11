# simple-NuGet-template
Here is an example for NuGet template creation, see article [How to create a template in .NET for a C# application and what NuGet is for](https://itnext.io/how-to-create-a-template-in-net-for-a-c-application-and-what-nuget-is-for-e5d4fc03c487)


**To create template open the command line and execute the following commands:**

C:\nuget.exe pack C:\Temp\SuperApp\SuperApp.ConsoleTemplate.CSharp.nuspec -OutputDirectory C:\Temp

dotnet new --install C:\Temp\SuperApp.ConsoleTemplate.CSharp.0.0.1.nupkg

dotnet new shwa -o C:\Temp\MyApp

cd C:\Temp\MyApp

dotnet run

![image](https://user-images.githubusercontent.com/40200852/121666986-83410d00-cab2-11eb-9246-f467b914b60a.png)

![image](https://user-images.githubusercontent.com/40200852/121667039-8c31de80-cab2-11eb-9400-4c115115f850.png)

![image](https://user-images.githubusercontent.com/40200852/121667062-93f18300-cab2-11eb-8971-b9646ed65f9f.png)

**So, what we did with these commands?**

we packed the template to NuGet package by the instructions provided in the .nuspec file
then we installed the template from the NuGet package to the dotnet, we need to check it works
we created an application from the newly installed template
then we ran it to check that it works
lastly, we see that console output, the folder and application renamed to the new name we provided in the command
