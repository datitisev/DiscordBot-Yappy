# Setting Up

<warn>
Keep in mind these are the instructions for the beta.
If you are not using the beta, please set the URL to https://www.yappybots.tk.
This message will be removed when the beta goes live.
</warn>

Follow the following steps to set up Yappy with any repo on Github.

**Discord**
1. Go to the channel you want events in for a repo
2. Say `G! init REPO`, where `REPO` can be `username/repo`, a github url.. more usage info at `GL! help init`
  - If the repository is private, make sure you tell Yappy that with `GL! init REPO private`;

**Github**
1. Go to the Github repo you want to have events for
2. Click Settings > Webhooks
3. Set `URL` to https://www.yappybots.tk/github
4. Set `Content-Type` to whatever you prefer, Yappy supports both `application/json` and `application/x-www-form-urlencoded`.
5. Select the events you want to emit to the channel
6. Click "Add Webhook"

Now you can test the webhook by, in Settings > Webhooks, scrolling down the webhook, finding the webhook pointing to the url mentioned above, clicking it, and clicking the "Test" button on the right.
Keep in mind you will need to have a commit or two in the repo, as it will simulate a push request.