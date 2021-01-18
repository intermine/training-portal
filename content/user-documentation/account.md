# Account

You need to create a different account for each InterMine database you use; we hope to support single sign-on in the future. You can access your account from the top navigation bar. 

![](../../.gitbook/assets/account.png)

![](../../.gitbook/assets/account-form.png)

### How do I create an account?

You can create an account through the Login tab in the top navigation bar. Click on the "**I don't have an account**" link in the previous screenshot to register by entering a valid email address and a password. 

![](../../.gitbook/assets/create-account.png)

{% hint style="info" %}
Your account information is private and won't be accessible by other users or inspected beyond automatic performance optimisation and updates. You can read our [Privacy Policy](https://intermine.readthedocs.io/en/latest/about/privacy-policy/) for more details. 
{% endhint %}

### Profile

The account details tab allows you to set various aspects of your account as follows:

#### User preferences:

![](../../.gitbook/assets/user-preferences.png)

1. **Inform me by email of newly shared lists -** you can select✅ to receive an email if someone shares a list with you. 
2. **Allow other users to share lists with me without confirmation -** you can allow✅users to share lists with you without asking first. 
3. **Display name:** Set your public name displayed in your InterMine interface, which can be used when others share lists with you. 
4. **Your preferred email address:** Set the email address you prefer to use for correspondence - for example**,** if someone shares a list with you. This could be different from the email you use to login to your account. 
5. **The URL of your preferred Galaxy instance:** Results can be exported to [Galaxy](http://galaxyproject.org/) - see [Send results to the galaxy](https://flymine.readthedocs.io/en/latest/results-tables/Documentationresultstables.html#resultsgalaxy). By default the main galaxy server is set; however, if you routinely use another galaxy instance, you can set this to be the default.

Make sure to click **Save Changes** to update your user settings.

{% hint style="info" %}
Sharing lists is not yet implemented in the BlueGenes interface. However, if you set your email preferences here, they will be relevant should you use the old interface. We hope to implement the sharing lists feature in BlueGenes soon.
{% endhint %}

#### Change password:

![](../../.gitbook/assets/password.png)

You can change your password using the Change password form shown in the previous screenshot. You just need to type in your old and new passwords and click Save Password to update your password. 

#### Delete account: 

![](../../.gitbook/assets/delete-account%20%281%29.png)

![](../../.gitbook/assets/delete-account-code.png)

To delete your account, you can click **Start Account Deletion**, which will direct you to a confirmation page. You need to copy and paste the confirmation code in the provided input field and click **Delete Account**. Once completed, you will no longer be able to login to your account and access your content and user preferences on this InterMine instance.

{% hint style="danger" %}
Account deletion cannot be undone. 
{% endhint %}

**API access key:**

API keys are used to access the features of the [InterMine API](https://intermine.readthedocs.org/en/latest/web-services/) without having to use your username or password.

### Are my lists and searches stored permanently?

Yes. When you have a MyMine account any lists or queries you save are stored permanently.

### What happens to my lists and queries when you make a new database release?

All lists and queries are transferred to the new database release. Sometimes identifiers in lists become outdated and you will be asked to update your list \(see [I am being told to upgrade my lists - what does this mean?](https://flymine.readthedocs.io/en/latest/lists/overview/Documentationlists.html#listsupgrade)\). Occasionally we have to make changes to the underlying data model which make affect any queries you have saved. Please contact the relevant InterMine \([Contact Us](https://flymine.readthedocs.io/en/latest/contact/Documentationcontact.html#contact)\) if you would like any further information or help about such a query.

