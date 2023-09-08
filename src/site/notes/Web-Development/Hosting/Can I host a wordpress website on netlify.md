---
{"dg-publish":true,"permalink":"/web-development/hosting/can-i-host-a-wordpress-website-on-netlify/","dgPassFrontmatter":true,"created":"","updated":""}
---

🔺[[Web-Development/Hosting/Netlify\|Netlify]]

# Can I host a wordpress website on netlify
***
2023-06-11


> [!HAZARD] Quick answer 
> Yes it’s possible but no it probably wouldn’t be worth my time to do unless I needed to move everything off proprietary hosting 


## Can I host a wordpress website on netlify 

While Netlify is a great platform for hosting static websites, it does not currently support hosting WordPress websites out-of-the-box. WordPress is a dynamic CMS (Content Management System) that requires a server-side environment with a database to function properly.

However, it is possible to integrate Netlify with WordPress in a few different ways. One approach is to use a headless WordPress setup, where the WordPress CMS is used only for managing content and API endpoints, while the front-end website is built using a static site generator like Gatsby or Next.js and hosted on Netlify. This approach allows developers to leverage the benefits of both WordPress and Netlify.

Another approach is to use a third-party service like Shifter, which can convert a WordPress website into a static website that can be hosted on Netlify. However, this approach may not be suitable for all WordPress websites, as some features and functionality may not translate well to a static site.

In summary, while Netlify does not support hosting WordPress websites directly, there are ways to integrate Netlify with WordPress for specific use cases.
  
### How would I set this up if I did want to use Netlify and Wordpress together 

If you're interested in setting up a headless WordPress site with Netlify, here are the general steps you would need to follow:

1. Set up a WordPress site: You'll need to set up a WordPress site on a server that supports PHP and MySQL. There are many web hosting providers that offer WordPress hosting, or you can set up your own server using a tool like XAMPP or WAMP.

2. Install the WP REST API plugin: The WP REST API plugin allows you to access the WordPress data via API endpoints. Install and activate the plugin on your WordPress site.

3. Create your front-end site: Create your front-end site using a static site generator like Gatsby, which can pull data from the WordPress API. You can also use a CMS like Netlify CMS to manage content.

4. Deploy your site to Netlify: Once your front-end site is ready, deploy it to Netlify using the continuous deployment workflow. This will automatically rebuild and deploy your site whenever you push changes to your Git repository.

5. Configure your API endpoints: Configure your API endpoints to point to the WordPress site. You'll need to specify the WordPress site URL and API endpoints in your Gatsby configuration file or other static site generator configuration files.

6. Test your site: Test your site to make sure everything is working as expected. You should be able to see WordPress data being displayed on your front-end site.

Keep in mind that this is just a general overview of the steps involved, and the specifics will vary depending on your specific setup and requirements. It's recommended to consult with a web development professional if you're unsure about any aspect of the process.

#### Is this going to involve a lot of maintenance performing this setup and deployment? 

Setting up a headless WordPress site with Netlify can involve some initial maintenance and configuration, but once the site is up and running, it can be relatively low-maintenance. Here are some factors to consider:

1. WordPress updates: As with any WordPress site, you'll need to keep the core WordPress software and plugins up to date to ensure security and stability. This will require some ongoing maintenance.

2. Netlify updates: Netlify updates its platform regularly, and you may need to update your deployment configuration to take advantage of new features or fixes.

3. Server maintenance: If you're hosting your WordPress site on your own server, you'll need to handle server maintenance tasks like updates, backups, and security.

4. Content updates: You'll need to continue adding and updating content on your WordPress site, which may require ongoing maintenance.

Overall, while there is some maintenance involved in setting up and running a headless WordPress site with Netlify, it can be relatively low-maintenance compared to a traditional WordPress site, since you won't need to worry about server-side maintenance and scaling.

  

