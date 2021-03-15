

packetmanager snap is preinstalled on Ubuntu 20.04 LTS
https://snapcraft.io/docs/getting-started

Microsoft:
https://docs.microsoft.com/en-us/dotnet/core/install/linux-snap

- install dotnet sdk
sudo snap install dotnet-sdk --classic --channel=5.0
- register
sudo snap alias dotnet-sdk.dotnet dotnet


(sdk includes runtime !!)
- install runtime
sudo snap install dotnet-runtime-50 --classic
- register
sudo snap alias dotnet-runtime-50.dotnet dotnet


- export path
export DOTNET_ROOT=/snap/dotnet-sdk/current

-- 
And install visual studio code:
sudo snap install code --classic