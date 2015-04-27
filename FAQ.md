## FAQ ##

### Usage Instructions: ###
  1. Installl mono ipk onto your webos device
  1. Install mono ipk example
  1. Run Example, get a black card....mono is installed properly


### Where is mono installed to? ###
> Mono is installed to /media/cryptofs/apps/usr/palm/applications/com.engplayground.mono.webos.port/

### Where is the mono executable? ###
> $MONO\_HOME/bin/mono

### How to run your own .net compiled apps? ###
> In your app, include a startup script. An example can be downloaded from this site. In the startup script, run the mono executable with your apps execuatable as an argument. For example $MONO\_HOME/bin/mono YourApp.exe

### Can I create visual apps, using Mono? ###
> The mono port currently has SDL.NET included. It seems that SDL.NET works directly with the WebOS SDL library. In theory you can use SDL.NET to  create 2D and 3D apps. The current build of the mono port (version 0.0.2) has a broken libgdiplus library, which will create a black card when trying to use SDL.NET.

### Will you be including any Mono code changes on this site? ###
> This is an excellent question, there were code changes to get Mono to compile. Ultimately I'd like to submit more generic changes to the mono-project.org site itself. The changes I currently have in place are just to get a webos specific version of mono compiled, with little regard for code consistency, etc. I'd like to have a more platform "friendly" patch, before i release any source. I should be able to work on it right after libgdiplus gets working.