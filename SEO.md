
[https://dev.to/junko911/make-your-rails-application-seo-friendly-by-setting-meta-tags-6o5](https://dev.to/junko911/make-your-rails-application-seo-friendly-by-setting-meta-tags-6o5)

  

  

SEO friendly URL

a gem (or library) called friendly_id.

  

https://medium.com/la-revanche-des-sites/seo-ruby-on-rails-the-comprehensive-guide-2018-b4101cc51b78

  

Dynamic Error Pages

By default, Rails offers pages 404 (page does not exist or more), 422 (incomplete or incorrect resource) and 500 (server error) available in the / public directory. You will need to customize these pages to reflect the overall design of your site (with your layout / application.html.erb) or to dynamically return content based on the user.

  

However, if a search engine has already indexed your site, you will have to redirect your old pages, and therefore old URLs, to new ones so as not to lose your visitors on your 404 pages. In this case, you must create 301 redirects to specify that one page has been moved permanently to another.

The Rails routing system makes these 301 redirects quite easily in the routes.rb file:

  

  

Start by creating a meta.yml file in the config directory that will contain the default values:

  

The green_monkey gem makes it easy to integrate Microdata properties directly into your application:

  

Breadcrumb

The breadcrumb allows you to remember the location of a page on your site in the global tree. It is important in SEO since Google officially recommends to offer a breadcrumb on your website.

[breadcrumbs_on_rails](https://github.com/weppos/breadcrumbs_on_rails).

  

Sitemap

The sitemap is the file that contains the list of your website URL. This file is in XML format. It gives search engines information about your URL and the architecture of your site. It allows sites with a substantial content and a complex mesh to be better understood by search engines and thus be better referenced.

  

Robots.txt

The robots.txt file is a text file used for the natural referencing of your site, containing instructions for search engine indexing robots in order to specify which pages may or may not be indexed. You can visit robots-txt.com for more information about its contents.

  

AMP

Google AMP, for “Accelerated Mobile Pages” is a protocol designed by Google to enable a “faster web”. AMP pages are a variation of classic web pages with simplified HTML and JavaScript. AMP only keeps what is needed to display the information very quickly.

  

HTTPS

By default, if you have configured your server correctly with your SSL certificate, you should automatically have your Ruby On Rails application in HTTPS. To enable the feature for a specific environment, you will need to enable the following option:

  

  

Bonus

www to non-www redirection

In SEO, one of the recurring problems is the duplicate content, which corresponds to two different pages containing the same content. This problem is very often caused by the duplication of content between the non-www (http://example.com) and the www version ([http://www.example.com](http://www.example.com/)).

  

Cache

We explained in a previous article on the implementation strategies for SEO, the cache is not negligible especially if your site contains a lot of URLS. For each crawl of a site, Google’s robot dedicates a specific time. The faster your pages load, the more Google crawls pages on your site.

  

For compression, nothing more simple, just activate it with the middleware Rack :: Deflater. I

  

Homepage H1

In SEO, a page corresponds to a positioning goal. We usually include the company logo in the <h1> tag for the home page only (which uses the brand name as the alt attribute). All other pages on the site will have a relevant <h1> text tag on the page.

  

[https://www.inboundio.com/blog/seo-for-ruby-on-rails-complete-guide](https://www.inboundio.com/blog/seo-for-ruby-on-rails-complete-guide)

  

[https://tosbourn.com/ruby-on-rails-seo/](https://tosbourn.com/ruby-on-rails-seo/)

  

[https://devcamp.com/site_blogs/top-5-seo-tips-for-rails-applications](https://devcamp.com/site_blogs/top-5-seo-tips-for-rails-applications)

  

## **Make Sure Your Site Is Mobile Ready**

As more people use mobile devices than ever before, search engines are looking for ways to provide a better mobile experience. Google has already started assessing mobile friendliness when ranking sites. Fortunately, Rails makes it easy to optimize the mobile experience for users, thanks to the Mobile Fu gem. It 

  
  

DeviceDetector gem [https://github.com/podigee/device_detector](https://github.com/podigee/device_detector)

  
  

# Make your Rails app work offline. Part 1: PWA setup

  
  

https://alicia-paz.medium.com/make-your-rails-app-work-offline-part-1-pwa-setup-3abff8666194