
# Software Test Report




## I. Introdução

The purpose of this report is to present the results of the tests carried out on the "CodeLeap network" software developed by "codeleap" company.


## II. Testing Methodology.


The tests were performed according to the following methodology:

- Test type: Manual and automated tests

- Test strategy: Gray box

- Tools used: (React, cypress.io).






## III.  Test results

- Sign up: The user is able to log in after entering their name and clicking on "enter". ✅

- Post: The user is able to write a title and content, and after clicking "create", the publication becomes the most recent on the timeline. ✅

- Post: It is not possible to create a post without filling in the title and content. ✅

- Main screen: The user is able to edit and delete only their own posts. ✅

- Main screen: If the user tries to delete a post, a message is displayed to confirm whether the user is sure they want to delete the item. ✅

- Sign up/Main screen: Users with different names cannot edit or delete each other's posts. ✅

- Main screen: Upon refreshing the page, the user is prompted to return to the login page if they want to post, edit, or delete a publication. Only viewing remains free. ✅
## IV. Bugs and problems found


- Login: Upper or lowercase letters change the username, and it's possible to have 2 users with the same name (numbers and symbols are also allowed).

Image:

Imagem:
![App Screenshot](https://cdn.discordapp.com/attachments/896170579525246979/1103417117283455057/Captura_de_Tela_97.png)


- Login: It's possible to fill in the login with spaces only, and you can log in, but you're only allowed to view the posts.
Image:
![App Screenshot](https://media.discordapp.net/attachments/896170579525246979/1103419319985115227/20230503_173219.gif)


- Login: There is no character limit for the username. If a high number of characters are filled in, the main screen's front-end will break.
Image:
![App Screenshot](https://media.discordapp.net/attachments/896170579525246979/1103417116452982904/Captura_de_Tela_94.png?width=1211&height=671)

- Main screen: There is no character limit for the title and content, resulting in the same border breaking problem as before and increasing the page's horizontal dimension. If you edit the post, the dimensions remain the same, and only deleting the post will return the page to its normal size.
Image:

Imagem:
![App Screenshot](https://media.discordapp.net/attachments/896170579525246979/1103417115609927862/Captura_de_Tela_90.png?width=1413&height=671)

- Main screen: It's possible to create a post with no title or content if filled with spaces only. 

Image:

![App Screenshot](https://cdn.discordapp.com/attachments/896170579525246979/1103422765853319321/Captura_de_Tela_99.png)

- Main screen: The previously typed post is not deleted after being posted, and it can be reposted multiple times without a lock, potentially generating spam.
Image:


![App Screenshot](https://cdn.discordapp.com/attachments/896170579525246979/1103417116738212000/Captura_de_Tela_95.png)



## V. Conclusion

Based on the results obtained, we can conclude that the "CodeLeap network" software version demonstrated good performance in relation to the tests carried out. However, the problems found must be corrected before the final version is released.


## File used for testing

The file has not undergone many changes just a simple test using cypress was added

```bash
  https://drive.google.com/file/d/1r5OxOOYduFXRJFVAjlZvTSRIs9f-eFcw/view?usp=share_link
```

