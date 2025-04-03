# 4. Create an Admin Account

In this section, we'll create a Domain Admin account to use instead of the built-in administrator account.

## Create an Organizational Unit for Admins

1. Select **Start > Windows Administrative Tools > Active Directory Users and Computers**
2. ![](https://ik.imagekit.io/typeai/tr:w-1200,c-at_max/img_3jhyTefvfCScE81ycc.png){ width=400px }
3. Right-click on the Domain and select **New > Organizational Unit**
   - This is where we will store our admin account
4. ![](https://ik.imagekit.io/typeai/tr:w-1200,c-at_max/img_BAG6lFyxBiOprlWgVh.png){ width=400px }
5. Name the OU "Admins" and click **OK**
   - Uncheck 'Protect container from accidental deletion' (for lab purposes only)
6. ![](https://ik.imagekit.io/typeai/tr:w-1200,c-at_max/img_Swl38YcO3AeT12fKmt.png){ width=400px }

## Create the Admin User

1. Right-click the Admins Organizational Unit (OU) and select **New > User**
2. ![](https://ik.imagekit.io/typeai/tr:w-1200,c-at_max/img_sM6isGdeBoLAUe3YLL.png){ width=400px }
3. Enter the user's name in the required fields and click **Next**
4. ![](https://ik.imagekit.io/typeai/tr:w-1200,c-at_max/img_tdwCWHJcVOb7aukA3s.png){ width=400px }
5. Set a secure password
   - For lab purposes only:
     - Uncheck 'User must change password at next logon'
     - Check 'Password never expires'
   - Click **Finish**
6. ![](https://ik.imagekit.io/typeai/tr:w-1200,c-at_max/img_djcaMHcbUFjJAvAJxW.png){ width=400px }

## Add User to Domain Admins Group

1. Right-click the newly created user and select **Properties**
2. Select the **Member of** tab, then click **Add**
3. ![](https://ik.imagekit.io/typeai/tr:w-1200,c-at_max/img_BNudcrddsIwW63tfdi.png){ width=400px }
4. In the 'Enter the object names to select' field, type `domain admins` and click **Check Names**
5. ![](https://ik.imagekit.io/typeai/tr:w-1200,c-at_max/img_fVf4HkQkhaq9dz5wUe.png){ width=400px }
6. Click **OK**, then **Apply**, and finally **OK** to save changes and exit

## Test the New Admin Account

1. Sign out of the current Windows session
2. Log in using your newly created admin credentials Windows session
3. Log in using your newly created admin credentials
