# Installation - SDK and Runtime
wget https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb

sudo dpkg -i packages-microsoft-prod.deb

  sudo apt-get update; \
  sudo apt-get install -y apt-transport-https && \
  sudo apt-get update && \
  sudo apt-get install -y dotnet-sdk-3.1

sudo apt-get update; \
  sudo apt-get install -y apt-transport-https && \
  sudo apt-get update && \
  sudo apt-get install -y aspnetcore-runtime-3.1

sudo apt-get install -y dotnet-runtime-3.1

## creating a new project using CLI
   cd d:\
   
   cd dotnetcore/
   
   ls -l
   
   dotnet new console --name cApp1

   dotnet new classlib --name cl1
   
   ls -l
   
   cd cApp1/
   

   dotnet add reference --help
   
 
   cd cApp1/
   
   dotnet add reference ../cl1/cl1.csproj
   
   cd ..
   
   dotnet new classlib --name cl2
   
   dotnet add cApp1/cApp1.csproj reference cl2/cl2.csproj
   
   cat cApp1/cApp1.csproj
   
   ls -l
   
   dotnet new
   
   dotnet new sln --name mycoreSln
   ls  -l
   dotnet sln mycoreSln.sln add cApp1/cApp1.csproj cl1/cl1.csproj cl2/cl2.csproj
   cat mycoreSln.sln
   
  cd cApp1/
  
  dotnet add package Newtonsoft.Json --version 12.0.3

  ## build - root directory
  
   dotnet build

  ## RUN - root directory
  
  dotnet run --project cApp1/cApp1.csproj
  
  # sample sln commands
  
  - mysolution.sln
      - cl1
      
        - cl1.csproj
        
      - cl2
      
        - cl2.csproj
        
      - myConsoleApp
      
        - myconsoleapp.csproj
    
    
       dotnet new console --name myConsoleApp
   
   dotnet new classlib --name cl1
   
   dotnet new classlib --name cl2  


   dotnet.exe add myConsoleApp/myConsoleApp.csproj reference cl1/cl1.csproj cl2/cl2.csproj
   
   dotnet new sln --name mysolution
   
   dotnet sln mysolution.sln add myConsoleApp/myConsoleApp.csproj cl1/cl1.csproj cl2/cl2.csproj
   
   dotnet build
   
   dotnet.exe run --project myConsoleApp/myConsoleApp.csproj

    
  
   

  
  
