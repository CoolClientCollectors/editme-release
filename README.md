![kx5qTBT](https://user-images.githubusercontent.com/11377481/85215111-eab1fa00-b341-11ea-8b00-fb2a070d9e58.png)

Debunking the dev/users bs
First of all, the image above is complete lies. The "auth" which is pretty much a joke, stores some keys in an arraylist which are hwids and theyre compared against your HWID then it invokes exitJava if its not in that arraylist. The keys arent used for anything else if you look at the references to the 'KEYS' field its only used in the preInit method for "auth" and theres nothing thats encrypted by the keys themselves.
#
![image](https://user-images.githubusercontent.com/11377481/85233556-4aa5b080-b3d5-11ea-9937-e7ffbebc4e28.png)\


![](https://cdn.discordapp.com/attachments/702338689115619349/724272449159692308/image0.png)\
He also claims in this ss that he can put code in images? However looking at the assets in a hex editor u can see its just a normal png and theres no "code" in the images.\
![](https://i.imgur.com/bYLKq3I.png)\
User claiming theres probably a token logger. Anyone can disprove this with a bytecode viewer by searching for method references for openConnection or HttpUrlConnection and look at classes that contain references to it (The preInit method in the uncracked editme because i removed it from the cracked one, and some other methods for converting username to uuid with a API) or using Theia to find references to these methods. (https://github.com/Tigermouthbear/Theia) \
also according to the users/owners/whatever its custom base\
![image](https://user-images.githubusercontent.com/11377481/85234083-f7cdf800-b3d8-11ea-8597-44d350e3a591.png)\
but if it was a custom base idk why this class would be here\
![image](https://user-images.githubusercontent.com/11377481/85234104-16cc8a00-b3d9-11ea-8f49-d50637537520.png)

Lastly, here's a download of the uncracked jar if you want to look at it for yourself\
https://github.com/CoolClientCollectors/editme-release/raw/master/editme-notcracked.jar
