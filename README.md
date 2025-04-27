# 4. Create an Admin Account

In this section, we'll create a Domain Admin account to use instead of the built-in administrator account.

## Create an Organizational Unit for Admins

1. Select **Start > Windows Administrative Tools > Active Directory Users and Computers**
![](https://ik.imagekit.io/typeai/tr:w-1200,c-at_max/img_3jhyTefvfCScE81ycc.png)
2. Right-click on the Domain and select **New > Organizational Unit**
   - This is where we will store our admin account
![](https://ik.imagekit.io/typeai/tr:w-1200,c-at_max/img_BAG6lFyxBiOprlWgVh.png)
3. Name the OU "Admins" and click **OK**
   - Uncheck 'Protect container from accidental deletion' (for lab purposes only)
![](https://ik.imagekit.io/typeai/tr:w-1200,c-at_max/img_Swl38YcO3AeT12fKmt.png)

## Create the Admin User

1. Right-click the Admins Organizational Unit (OU) and select **New > User**
<img src=https://ik.imagekit.io/typeai/tr:w-1200,c-at_max/img_sM6isGdeBoLAUe3YLL.png width=400px>

2. Enter the user's name in the required fields and click **Next**

<img src=https://ik.imagekit.io/typeai/tr:w-1200,c-at_max/img_tdwCWHJcVOb7aukA3s.png width=400px >

3. Set a secure password
   - For lab purposes only:
     - Uncheck 'User must change password at next logon'
     - Check 'Password never expires'
   - Click **Finish**
<img src=https://ik.imagekit.io/typeai/tr:w-1200,c-at_max/img_djcaMHcbUFjJAvAJxW.png width=400px >

## Add User to Domain Admins Group

1. Right-click the newly created user and select **Properties**
2. Select the **Member of** tab, then click **Add**
<img src=https://ik.imagekit.io/typeai/tr:w-1200,c-at_max/img_BNudcrddsIwW63tfdi.png width=400px >
3. In the 'Enter the object names to select' field, type `domain admins` and click **Check Names**
<img src=https://ik.imagekit.io/typeai/tr:w-1200,c-at_max/img_fVf4HkQkhaq9dz5wUe.png width=400px >
4. Click **OK**, then **Apply**, and finally **OK** to save changes and exit

## Test the New Admin Account

1. Sign out of the current Windows session
2. Log in using your newly created admin credentials
