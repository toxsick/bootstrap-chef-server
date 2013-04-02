# Usage

This is a helper kitchen for knife solo for bootstraping a chef server



First pepare the target node:
	
	knife solo prepare user@address
	
After that an node json has been created in the /nodes folder. Replace the content with:

	{
  		"run_list": [
    		"recipe[chef-server]"
  		]
	}
	
Finally run cook:

	knife solo cook user@address

Type in the servers password a few times and you should be up and running.

The WebUI schould be reachable unter

	https://se.rv.er.ip
	
