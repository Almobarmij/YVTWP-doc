YVTWP (Youtube Videos To Wordpress Posts) plugin allows users to import Youtube videos to Wordpress in the easiest possible way. The documentation will take you through the list of available options.

##Setting Your Google Developer Key

Before you start using the plugin, you must get a Google API key. Navigate to the `Youtube API Settings` menu, follow the instructions to get your API key and paste it on the `Developer Key` input.

##Plugin Dashboard

The plugin dashboard shows the list of imports with the pagination and filter options. You can see more details about the import by clicking the `Load feed` link.

![Imports list](https://dl.dropboxusercontent.com/s/vmkasnxcbsdk2af/Screenshot%202015-09-02%2014.21.04.png?dl=0)

To minimize the number of API requests, we implemented a caching system for results. You can clear the cache by clicking on the `Clear Cache` link on list items.
When you remove an import, the list of posts you imported are also going to be removed from Wordpress. Make sure that you don't remove any existing data.

##New Import

You can create new imports from the `New Import` link. You have the option to import channels videos, playlists, user videos, search using a query, single video. Before exploring each import type, lets talk more about option tabs.

###Feed Options

The feed options tab is where you're going specify your feed details. Most fields are self explanatory, but some are Not :)
Bulk import allows you to import all the results of this import directly without seeing the list of videos. This is useful when importing a playlist or channel.
Advanced video filter allows you to filter down videos using video definition, duration, category, etc. This option is only available for channel and search query imports.

###General Options

The general options tabs specify how videos are integrated into Wordpress. You can import videos as posts, pages, attachments, etc. You can also specify post status, author (post owner) and how video thumbnail is imported. You can specify if you want to update a post if it was already imported.

###Embed Options

The embed options tab specify how videos are inserted into Wordpress, you can create the necessary markup and inject variable like `video_key`, `video_url`, etc. The bottom section is used to map those variable to custom fields, this option can be useful if you're using a video theme.

###Title & Description Options

The title and description options allow you to perform transformation to the title and the description by removing, adding and replacing keywords from the text.

###Scheduling options

As the name suggest, these options are useful for scheduling videos posting. You need to activate it by selecting `Yes` on the `Activate post scheduling`, and then you can select the starting date and time and time interval between each post.

*Note:* You can set `Random min value` and `Random max value` to the same value if you want a fixed margin time between posts.

##Default Import Settings

The `Default Import Settings` page will save you the time of typing the same details every time you want to perform a new import.


##Importing Feed

After selecting the feed type and filling tabs accordingly, you can click `Save and Import feed` to start the import. This will show the list of found videos (except for single video import) with pagination if necessary. If you chose to do a bulk import, you'll be redirected the a screen showing the import progress.

If a video already exists, it will have a label next to the video title. You can also customize which video details you want to show on screen and how many videos to use for the pagination.

The below video shows a demo on the basic plugin usage.

// video here

