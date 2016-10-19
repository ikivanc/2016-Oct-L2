# Create a pair of SSH keys using Bash (For Mac, Linux and Windows 10 with Bash installed)
1. Use *'ssh-keygen'* to create an RSA SSH key of 4096 bits pointing to our e-mail address.
    
    ```Shell
    ssh-keygen -t rsa -b 4096 -C "mymail@brus.ml"
    ```

1. After this command you will be asked for a location to save your powerful key, you can give it a custom location but it's not really necessary unless you actually handle multiple keys.

    ```Shell      
    Enter a file in which to save the key (/Users/you/.ssh/id_rsa): [Press enter]
    ```

2. Now you will be asked to enter a password to increase the level of security of your key. This password is optional, but if you decide to set it up you will need to enter it every time you interact with your SSH private key:

    ```Shell
        Enter passphrase (empty for no passphrase): [Type a passphrase]
        Enter same passphrase again: [Type passphrase again]
    ``` 

3. Now, after your key was created just *cat* the content of your public key (if you used a different location, make sure you use the correct file). This is the 

```Shell
    code ~/.ssh/id_rsa.pub
    [This is an example of how and your pub key should look like:]
    ssh-rsa 123456789/dTc6wJT+YCOUiLLS6F7Ge4WlCgmH7fW7UIUJpFcXwDv1bWVMQ3chBFFELWEhEjCqX7HAVoSjEF8oAwM0Ik5p6y66J420eeOGBLHkyV+nBiV0F5WVRKFS5Az1rZy8x/1usbMms/skMnS5Int9QcGIIA9g7Ws9xg28/2XA5IUPUZ0kIKbuSv7bAIqrHaH7WXzUeLeOjUIeW34d9WO52kNqiITjyW1D7kThXKtgS9Y5TEie5MuP8plzz+mBID59EFmdEhBK7QquuT6axI1PIDNm4PrhI7mJP9IgRRQOOXZ1rvoysOHxhDvzVWRuc623pV8PPjiBHiu1Y1T mymail@brus.ml
```
