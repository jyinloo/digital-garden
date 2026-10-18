2026-10-17 14:06

Status: 

Tags: #digitalgarden #howto

## A guide to publishing Obsidian for free

1. Download https://nodejs.org/en
2. Go to https://github.com/jackyzha0/quartz
3. Click `Use this template` > `Create a new repository`
4. Rename repository 
5. In the Terminal window type the following:  
`git clone https://github.com/<jyinloo>/<your-repo>.git`
Replace the address with the address from your github. You can get this address by clicking `<> Code` under **HTTPS**

6. Enter the following code in your Terminal window  
`cd gardenexample`

7. Enter the following code in your Terminal window  
`npm i   `If any errors come up, make sure you downloaded [https://nodejs.org/en](https://nodejs.org/en)

8. Then enter:  
`npx quartz create`

9. You’ll see options:
    - Choose `Obsidian` as your template.
        
    - Choose `Copy an existing folder`.
        
    - Enter the file path to your Obsidian vault
        
        - To grab the file path, open your Finder window and locate your Obsidian vault location.
            
        - If you don’t know where it is, you can open Obsidian, and on the bottom-left of your window click the two arrows and click **Manage Vaults**.
            
        - Click the three dots > **Reveal vault in Finder**
            
        - Drag and drop the Vault folder to your terminal. Click enter
            
    - Enter your base URL: `mysite.github.io/quartz`
        
        - Mine was `margaretalba.github.io/gardenexample`
        
10. Enter the base URL for your Quartz site:  
    I used `margaretalba.github.io/gardenexample`
#### Install plugins

 Then enter:  
`npx quartz plugin install --from-config`


#### Publishing

 To publish your site enter the following in your terminal:  
`npx quartz sync --no-pull`

From now on, if you need to update your site, you can enter
`npx quartz sync`


**You can now see your site at http://localhost:8080**
## References
https://margaretalba.substack.com/p/a-non-technical-guide-to-publish