YVTWP (Youtube Videos To Wordpress Posts) plugin allows users to import Youtube videos to Wordpress in the easiest possible way. The documentation will take you through the list of available options.

##Setting Your Google Developer Key

Before you start using the plugin, you must get a Google API key. Navigate to the `Youtube API Settings` menu, follow the instructions to get your API key and paste it on the `Developer Key` input.

###Steps
After signing to Google account, navigate to the [Developer Console](https://console.developers.google.com/project) and click on the `Create Project` button.

![Create Project](https://dl.dropboxusercontent.com/s/8iy2oc50gn18k7m/Screenshot%202015-09-02%2012.31.52.png?dl=0)

Give your project a name and click `create`. Now you can select your project from the list at the top of the window.

![Choose Project](https://dl.dropboxusercontent.com/s/xr5jtwxhdc8x017/Screenshot%202015-09-02%2013.25.53.png?dl=0)

The left menu contains an `APIs & auth` menu where you can activate Youtube API if it's not activated by default.

![Activate Youtube API](https://dl.dropboxusercontent.com/s/ea79aa10gm2xjrj/yvtwp_activate_api.gif?dl=0)

Select `credentials and create a new API key.

![Create API Key](https://dl.dropboxusercontent.com/s/dxy58c57qws6nqf/yvtwp_create_key.gif?dl=0)

##Plugin Dashboard

The plugin dashboard shows the list of imports with the pagination and filter options. You can see more details about the import by clicking the `Load feed` link.

![Imports list](https://dl.dropboxusercontent.com/s/vmkasnxcbsdk2af/Screenshot%202015-09-02%2014.21.04.png?dl=0)

To minimize the number of API requests, we implemented a caching system for results and it's cleared whenever you change the import options. You can clear the cache by clicking on the `Clear Cache` link on list items.
When you remove an import, the list of posts you imported are also going to be removed from Wordpress. Make sure that you don't remove any existing data.

##New Import

You can create new imports from the `New Import` link. You have the option to import channels videos, playlists, user videos, search using a query, single video. Before exploring each import type, lets talk more about option tabs.

![New Import](https://dl.dropboxusercontent.com/s/dvss0hrki3dhhjo/Screenshot%202015-09-03%2012.39.24.png?dl=0)

###Feed Options

The feed options tab is where you're going to specify your feed details. Most fields are self explanatory, but some are Not :)
Bulk import allows you to import all the results of this import directly without seeing the list of videos. This is useful when importing a playlist or channel.
Advanced video filter allows you to filter down videos using video definition, duration, category, etc. This option is only available for channel and search query imports.

![Feed Options Tab](https://dl.dropboxusercontent.com/s/8rp2iwinqpamzei/Screenshot%202015-09-04%2011.10.28.png?dl=0)

###General Options

The general options tabs specify how videos are integrated into Wordpress.

- You can import videos as posts, pages or any custom post type. 
- Specify post status, author (post owner) and how video thumbnail is imported.
- Specify if you want to update a post if it was already imported.
- Import Youtube categories, and assign post to any existing category. Same thing goes for tags.

![General Options](https://dl.dropboxusercontent.com/s/ugitjx8zaprfwy0/Screenshot%202015-09-04%2011.11.23.png?dl=0)

###Embed Options

The embed options tab specify how videos are inserted into Wordpress, you can create the necessary HTML markup and inject variables like `video_key`, `video_url`, `video_description`, `video_title`, etc. You can also use the `[yvtwp_video]` shortcode to simply add the Youtube video iframe. The bottom section is used to map those variable to custom fields. This option lets you easily integrate imported videos into your theme.

![Feed Options Tab](https://dl.dropboxusercontent.com/s/hpm9liai5oj5uj1/Screenshot%202015-09-04%2011.14.06.png?dl=0)

###Title & Description Options

The title and description options allow you to perform transformation to the title and the description by removing, adding and replacing keywords from the text.

![Title Options Tab](https://dl.dropboxusercontent.com/s/b7duwza2exijgnc/Screenshot%202015-09-04%2011.15.14.png?dl=0)

![Description Options Tab](https://dl.dropboxusercontent.com/s/f0quhd51dnzdyzj/Screenshot%202015-09-04%2011.16.17.png?dl=0)

###Scheduling options

As the name suggest, these options are useful for scheduling videos posting. You need to activate it by selecting `Yes` on the `Activate post scheduling`, and then you can select the starting date and time and time interval between each post.

    *Note:* You can set `Random min value` and `Random max value` to the same value if you want a fixed margin time between posts.

![Scheduling Options Tab](https://dl.dropboxusercontent.com/s/c7p9xtl36hec1wj/Screenshot%202015-09-04%2011.16.57.png?dl=0)

##Default Import Settings

The `Default Import Settings` page will save you the time of typing the same details every time you want to perform a new import.

![Default Import Settings](https://dl.dropboxusercontent.com/s/qspbaxbuzyzb5g0/Screenshot%202015-09-04%2011.33.18.png?dl=0)

##Importing Feed

After selecting the feed type and filling tabs accordingly, you can click `Save and Import feed` to start the import. This will show the list of found videos (except for single video import) with pagination if necessary. If you chose to do a bulk import, you'll be redirected the a screen showing the import progress.

If a video already exists, it will have a label next to the video title. You can also customize which video details you want to show on screen and how many videos to use for the pagination.

![Import result](https://dl.dropboxusercontent.com/s/unm1v1maqt7y3oh/Screenshot%202015-09-03%2012.23.03.png?dl=0)

The below video shows a demo on the basic plugin usage.

// video here

##Key Features

- Youtube API v3
- Multiple feed types integration. (single video, channel, user, playlists, search query)
- Powerful caching system.
- Bulk import.
- Result filter support (for playlists and search queries).
- Custom post types integration.
- Scheduled posting.
- Flexible embed options for your theme.
- Default settings for easier import.

##Screenshots

![Import result](https://dl.dropboxusercontent.com/s/unm1v1maqt7y3oh/Screenshot%202015-09-03%2012.23.03.png?dl=0)

![Bulk Import](https://dl.dropboxusercontent.com/s/g10todl8k0wbrop/Screenshot%202015-09-04%2011.32.19.png?dl=0)

![Imports](https://dl.dropboxusercontent.com/s/muy89loay6x40hx/Screenshot%202015-09-03%2013.00.00.png?dl=0)

![Schedule Options](https://dl.dropboxusercontent.com/s/8oqxrb4h2vxmxnv/Screenshot%202015-09-04%2011.37.34.png?dl=0)

![Youtube API Settings](https://dl.dropboxusercontent.com/s/ykz5bodfd8px94j/Screenshot%202015-09-04%2011.38.31.png?dl=0)
