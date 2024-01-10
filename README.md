# Bastille-webtrees
webtrees is a web application that allows you to publish your genealogy online, collaborate with family members and take control of your data.

Install webtrees in a FreeBSD jail BastilleBSD
Installation overview using XigmanasNAS Bastille Extension Gui

## Jail Setup
1. From the main screen select Extension/Bastille

2. Click ADD [+] button

3. Name (any name will work): webtrees

4. Configure Network Properties to your liking

5. Base Release: 12.3-Release (or newer)

6. Jail Type: 
- [ ] Create a thick container.
- [x] Enable VNET(VIMAGE).
- [ ] Create an empty container.
- [x] Start after creation.
- [x] Auto start on boot.

7. Click Create

8. Click Save

9. Restart the jail.


## Applying the Firefly template to the newly created jail

1. SSH to your Xigmanas Server

2. BOOTSTRAP the dependency template
`bastille bootstrap https://github.com/DarkenLight/Bastille-nginx`

3. BOOTSTRAP the webtrees template
`bastille bootstrap https://github.com/DarkenLight/Bastille-webtrees`

4. Apply the Template to the TARGATE jail.
`bastille template webtrees DarkenLight/Bastille-webtrees`


## Thanks to Webtrees Developer
https://github.com/webtrees
