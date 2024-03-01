# WP.IntroductionResources

## Key concepts

- **[WordPress Core Architecture](#WordPress-core-architecture)**: Understanding the core architecture, including the main directories (wp-admin, wp-includes, wp-content), core files, and how WordPress serves content.

- **[Themes](#Theme-development) and [Plugins](#plugins)**: Knowledge of how to create and customize themes and plugins, including understanding the template hierarchy, hooks (actions and filters), and the WordPress Loop.

- **[Custom Post Types and Taxonomies](#Custom-Post-Types-and-Taxonomies)**: Creating custom post types and taxonomies to extend WordPress content management capabilities beyond posts and pages.

- **[WordPress REST API](#wordpress-rest-api)**: Utilizing the WordPress REST API for creating custom endpoints or interfacing WordPress with external applications, allowing for headless CMS architectures.

- **Security and Performance Optimization**: Implementing best practices for securing WordPress sites, including data validation/sanitization, and strategies for optimizing site performance (caching, database optimization, image compression). ==> **_This is usually PhiLac that manages that part so you have less to worry here_**

- **[Docker+WorPress](Docker+WordPress)**. To ease the development process, having docker as part of the tooling could be quite important.

## WordPress core architecture

Most of the work will likely be done in the wp-content/theme folder while creating our own theme. It would happen that for certain project, we need to create our own plugin OR extension for the wp-admin.

Most of the content and the best resource is the WordPress developer resource [here](https://developer.wordpress.org/themes/core-concepts/)

One of the most common resource used is the page hierachy form WordPress. So you can refer to this link [here](https://developer.wordpress.org/themes/basics/template-hierarchy/)

![par hierachy](https://i0.wp.com/developer.wordpress.org/files/2014/10/Screenshot-2019-01-23-00.20.04.png?ssl=1)

#### Top 10 Links to Learn About WordPress Core Architecture

1. [WordPress Architecture - WordPress Codex](https://codex.wordpress.org/WordPress_Architecture) - The official WordPress Codex page detailing the WordPress architecture.
2. [WordPress Developer Resources - Code Reference](https://developer.wordpress.org/reference/) - Official WordPress developer documentation, including code reference for understanding core architecture.
3. [Understanding WordPress Core Architecture - Smashing Magazine](https://www.smashingmagazine.com/2021/03/complete-guide-wordpress-architecture/) - A comprehensive guide on WordPress architecture by Smashing Magazine.
4. [WordPress Core Architecture - WPBeginner](https://www.wpbeginner.com/glossary/core/) - WPBeginner offers an easy-to-understand overview of WordPress core.
5. [Inside WordPress Core - SitePoint](https://www.sitepoint.com/inside-wordpress-core/) - SitePoint's deep dive into the WordPress core, explaining its fundamental components.
6. [Exploring the WordPress File and Directory Structure - Elegant Themes](https://www.elegantthemes.com/blog/wordpress/wordpress-file-and-directory-structure) - Elegant Themes explains the file and directory structure of WordPress.
7. [The WordPress Database Structure - CodeinWP](https://www.codeinwp.com/blog/wordpress-database-structure/) - CodeinWP's detailed look at the WordPress database structure.
8. [How WordPress Works Behind the Scenes - WPBeginner](https://www.wpbeginner.com/beginners-guide/how-wordpress-actually-works-behind-the-scenes/) - A beginner-friendly guide on how WordPress works behind the scenes by WPBeginner.
9. [Understanding the WordPress Core Software - TutsPlus](https://code.tutsplus.com/tutorials/understanding-the-wordpress-core-software--wp-25446) - TutsPlus tutorial on understanding the WordPress core software.
10. [WordPress Structure - ThemeShaper](https://themeshaper.com/2012/02/13/understanding-the-wordpress-file-and-directory-structure/) - ThemeShaper's guide to understanding WordPress file and directory structure.

## Theme development

Creating a theme in WordPress allows for unparalleled customization and control over a website's appearance and functionality, enabling developers and designers to craft unique user experiences tailored to specific needs or branding requirements. A custom theme can integrate specific design elements, functionality, and optimizations that pre-built themes may not offer, providing a more cohesive and optimized user experience. Additionally, developing a theme from scratch or customizing an existing one helps in understanding WordPress's core functionality and architecture, enhancing one's skills in web development within the WordPress ecosystem.

However, there are several "gotchas" to be mindful of. Ensuring compatibility with the latest WordPress core updates is crucial to maintain the site's functionality and security. Developers must adhere to WordPress coding standards and best practices to ensure their theme is efficient, secure, and scalable. Over-customization without proper enqueueing of scripts and styles can lead to conflicts with plugins and core updates. Lastly, neglecting responsive design or accessibility standards can severely impact user experience and site performance. Balancing custom functionality with performance optimization and maintaining code readability and documentation are key considerations for successful WordPress theme development.

#### Top 10 Links for Creating and Developing Themes in WordPress

1. [Theme Development - WordPress Codex](https://codex.wordpress.org/Theme_Development) - The official guide to theme development in WordPress.
2. [Theme Handbook - WordPress Developer Resources](https://developer.wordpress.org/themes/) - Comprehensive WordPress theme development handbook from the official WordPress Developer Resources.
3. [Developing a WordPress Theme from Scratch - Tania Rascia](https://www.taniarascia.com/developing-a-wordpress-theme-from-scratch/) - A step-by-step guide to creating a WordPress theme from scratch.
4. [How To Create And Customize A WordPress Child Theme - Smashing Magazine](https://www.smashingmagazine.com/2016/01/create-customize-wordpress-child-theme/) - Smashing Magazine’s tutorial on creating and customizing a WordPress child theme.
5. [WordPress Themes In Depth - DigWP](https://digwp.com/book/) - A comprehensive book and resource for developing WordPress themes in depth.
6. [Building Custom WordPress Theme - Web Designer Wall](https://webdesignerwall.com/tutorials/building-custom-wordpress-theme) - A tutorial on building custom WordPress themes with a focus on design.
7. [UnderStrap WordPress Theme Framework](https://understrap.com/) - A WordPress theme framework that combines the Underscores starter theme and Bootstrap.
8. [A Guide to Overriding Parent Theme Functions in Your Child Theme - WPBeginner](https://www.wpbeginner.com/wp-themes/how-to-override-parent-theme-functions-in-wordpress/) - WPBeginner's guide to overriding parent theme functions in child themes.
9. [Creating a WordPress Theme From Static HTML: Preparing the Markup - Envato Tuts+](https://webdesign.tutsplus.com/series/creating-a-wordpress-theme-from-static-html--webdesign-20467) - A series on converting static HTML to a fully functional WordPress theme.
10. [Advanced WordPress Theme Development with Bootstrap 4 - Udemy](https://www.udemy.com/course/advanced-wordpress-theme-development-with-bootstrap-4/) - An online course for advanced WordPress theme development using Bootstrap 4.

These resources range from official documentation to comprehensive tutorials and courses, providing valuable knowledge for both beginners and experienced theme developers in the WordPress ecosystem.

## Plugins

A majority of the sites we build would be using a combination of the below plugins as a "Core" set of plugins for development.

- **ACF and ACF PRO**: Enhances WordPress with advanced custom fields and powerful field management.

- **Elementor**: A drag-and-drop page builder for WordPress, enabling easy site design.

- **WPBakery**: A page builder plugin for WordPress, offering front-end and back-end editing.

- **Contact Form 7**: Simple but flexible contact form plugin, with customizable form and mail content.

- **Yoast**: A comprehensive SEO plugin, offering analysis and optimization for WordPress content.

### Other used plugins

- **WPML**: A plugin enabling multilingual content management in WordPress, supporting translations across posts, pages, and taxonomies.

- **WP Multisite**: A WordPress feature that allows multiple virtual sites to share a single WordPress installation.

## Custom Post Types and Taxonomies

On most projects, we need to define custom post types to store specific bits of data (news, resources, recipes, locations...). Therefore understanding how to create, organize, store and interact with custom post types is **_very important_**

- **Using the WordPress `register_post_type()` and `register_taxonomy()` Functions**: Directly use WordPress's built-in functions in your theme's `functions.php` file or within a custom plugin to programmatically define custom post types and taxonomies.

- **Using a Plugin**: Utilize plugins like "Custom Post Type UI," "Toolset Types," or "Pods" to create and manage custom post types and taxonomies through a user-friendly interface without writing code.

- **Theme Integration**: Integrate custom post types and taxonomies directly into a theme, ensuring they are part of the theme's core functionality, offering a seamless experience tailored to the theme's design and purpose.

Two approaches that we usually prefer when it comes down to:

1. Register the post type using Custom Post Type UI and then create the post type fields in ACF
2. Register the post type directly in ACF and create the post type fields in ACF

But we would adapt this strategy based of: if we are creating a NET NEW SITE or INHERIT/MAINTAINING an existing site.

#### Top 5 Links for Creating Custom Post Types

1. [Post Types - WordPress Codex](https://codex.wordpress.org/Post_Types) - The official WordPress Codex page providing an overview of post types, including built-in and custom post types.
2. [Custom Post Types - WordPress Developer Handbook](https://developer.wordpress.org/plugins/post-types/) - Comprehensive guide on creating custom post types in the WordPress Developer Handbook.
3. [How to Create Custom Post Types in WordPress - WPBeginner](https://www.wpbeginner.com/wp-tutorials/how-to-create-custom-post-types-in-wordpress/) - A beginner-friendly tutorial on creating custom post types by WPBeginner.
4. [Creating Custom Post Types with Plugins vs Functions.php - Torque](https://torquemag.io/2015/07/creating-custom-post-types-plugins-vs-functions-php/) - A comparison of creating custom post types using plugins versus the theme’s functions.php file by Torque.
5. [A Guide to WordPress Custom Post Types: Creation, Display and Meta Boxes - Smashing Magazine](https://www.smashingmagazine.com/2012/11/complete-guide-custom-post-types/) - An in-depth guide on creating custom post types, displaying them, and working with meta boxes by Smashing Magazine.

## WordPress REST API

The WordPress REST API is a powerful tool that enables developers to interact with WordPress sites remotely by sending and receiving JSON (JavaScript Object Notation) objects. This API facilitates the development of headless WordPress architectures, where the backend (WordPress) is decoupled from the frontend presentation layer, allowing developers to use any technology stack for the frontend while leveraging WordPress's robust content management capabilities in the backend.

The WordPress REST API is a powerful tool that enables developers to interact with WordPress sites remotely by sending and receiving JSON (JavaScript Object Notation) objects. This API facilitates the development of headless WordPress architectures, where the backend (WordPress) is decoupled from the frontend presentation layer, allowing developers to use any technology stack for the frontend while leveraging WordPress's robust content management capabilities in the backend.

### Advantages:

- **Flexibility**: Enables the use of WordPress as a headless CMS with any frontend technology.
- **Accessibility**: Simplifies external applications' access to WordPress content and functionalities.
- **Development Efficiency**: Streamlines the development process, offering standardized endpoints for posts, users, categories, etc.

### Inconveniences:

- **Security Concerns**: Exposes a public API that could be a target for unauthorized access if not properly secured.
- **Complexity**: Requires a good understanding of RESTful principles and authentication mechanisms.
- **Performance**: Can introduce additional latency, especially if not properly cached or optimized, due to the overhead of HTTP requests.

#### Top 5 Links for Learning About the WordPress REST API

1. [WordPress REST API Handbook](https://developer.wordpress.org/rest-api/) - The official handbook for the WordPress REST API, providing comprehensive documentation on using and extending the REST API.

2. [An Introduction to the WordPress REST API - WPBeginner](https://www.wpbeginner.com/wp-tutorials/wp-rest-api-beginners-guide/) - A beginner-friendly guide to understanding and using the WordPress REST API.

3. [Using the WordPress REST API with JavaScript - Smashing Magazine](https://www.smashingmagazine.com/2018/03/using-the-wordpress-rest-api-with-javascript/) - Smashing Magazine's tutorial on how to use the WordPress REST API in conjunction with JavaScript.

4. [The WordPress REST API: What It Is and How to Get Started Using It - Torque](https://torquemag.io/2015/07/working-with-the-wordpress-rest-api/) - A Torque article explaining what the WordPress REST API is and how to start using it in your projects.

5. [Headless WordPress: Using WordPress as a Headless CMS with the REST API - CSS-Tricks](https://css-tricks.com/headless-wordpress-using-wordpress-as-a-headless-cms/) - CSS-Tricks explores using WordPress as a headless CMS with the REST API, including practical examples and considerations.

## Docker+Wordpress

Using Docker for WordPress development offers an efficient, scalable, and consistent environment for building and testing websites. It simplifies the process of configuring development environments, ensuring that developers can work in an isolated setup that mirrors production settings without the hassle of manual configurations. Docker containers can run WordPress, associated services like MySQL and PHP, and tools for development and debugging, ensuring compatibility across different machines and teams. This approach reduces "it works on my machine" problems, streamlining development, testing, and deployment processes across various environments.

### Top 10 Links and Resources for WordPress Development with Docker

1. [Docker Official WordPress Image](https://hub.docker.com/_/wordpress/) - Official Docker image for WordPress.
2. [WordPress Development with Docker Compose](https://css-tricks.com/wordpress-development-with-docker-compose/) - A guide on CSS-Tricks for setting up WordPress with Docker Compose.
3. [Using Docker for WordPress Development](https://deliciousbrains.com/docker-wordpress-development/) - An introduction by Delicious Brains.
4. [Docker + WordPress: A Perfect Match](https://www.smashingmagazine.com/2021/06/docker-wordpress-local-development/) - Smashing Magazine’s guide to using Docker for local WordPress development.
5. [Setting Up Docker for WordPress Development](https://wptavern.com/setting-up-docker-for-wordpress-development) - WP Tavern’s tutorial on Docker for WordPress.
6. [Dockerize WordPress](https://www.sitepoint.com/dockerize-wordpress/) - A SitePoint tutorial for Dockerizing WordPress.
7. [Local WordPress Development with Docker](https://themeisle.com/blog/local-wordpress-development-with-docker/) - Themeisle’s comprehensive guide to local development with Docker.
8. [Developing WordPress Sites with Docker](https://torquemag.io/2021/03/developing-wordpress-sites-with-docker/) - Torque Mag’s insights into Docker-based development.
9. [How to Use Docker for Easy and Fast WordPress Development](https://kinsta.com/blog/wordpress-docker/) - Kinsta’s take on Docker for WordPress development.
10. [WordPress Development Environment with Docker](https://www.codeinwp.com/blog/wordpress-development-environment-docker/) - CodeinWP’s guide to setting up a Docker-based environment.
