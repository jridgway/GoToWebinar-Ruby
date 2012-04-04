#GoToWebinar

This is a project to build a Ruby wrapper for using Citrix's GoToWebinar REST API. 

##Requirements

You must have an active GoToWebinar account and a valid access token from the GoToWebinar OAuth flow. Please refer to the [authentication and authorization documentation](https://developer.citrixonline.com/page/authentication-and-authorization). 

##Install

It isn't an official repository yet so you can't do the normal gem install route.

	gem install go_to_webinar
	
For now you will need to install from source. 

	gem install go_to_webinar, :git => 'git://github.com/nathanwfish/GoToWebinar.git'

##Usage

Please refer to the [developer documentation](https://developer.citrixonline.com/api-overview/gotowebinar-rest-api) for a complete list of available methods. 

	@g2w = GoToWebinar::API.new(oauth_access_token) 
	@g2w.get_webinar(organizer_key, webinar_key)

##Status

Tests are incomplete at this time. 
