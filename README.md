# ![LOGO](logo.png) Gitea API. **flow**ground Connector

## Description

A generated **flow**ground connector for the Gitea API. API (version 1.1.1).

Generated from: https://api.apis.guru/v2/specs/gitea.io/1.1.1/swagger.json<br/>
Generated at: 2019-05-07T17:40:57+03:00

## API Description

This documentation describes the Gitea API.

## Authorization

Supported authorization schemes:
- API Key- API Key- Basic Authentication
- API Key- API Key- API Key
## Actions

### List all organizations

*Tags:* `admin`

### List all users

*Tags:* `admin`

### Create a user

*Tags:* `admin`

### Delete a user

*Tags:* `admin`

#### Input Parameters
* `username` - _required_ - username of user to delete

### Edit an existing user

*Tags:* `admin`

#### Input Parameters
* `username` - _required_ - username of user to edit

### Add a public key on behalf of a user

*Tags:* `admin`

#### Input Parameters
* `username` - _required_ - username of the user

### Delete a user's public key

*Tags:* `admin`

#### Input Parameters
* `username` - _required_ - username of user
* `id` - _required_ - id of the key to delete

### Create an organization

*Tags:* `admin`

#### Input Parameters
* `username` - _required_ - username of the user that will own the created organization

### Create a repository on behalf a user

*Tags:* `admin`

#### Input Parameters
* `username` - _required_ - username of the user. This user will own the created repository

### Render a markdown document as HTML

*Tags:* `miscellaneous`

### Render raw markdown as HTML

*Tags:* `miscellaneous`

### Create a repository in an organization

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of organization

### Create an organization

*Tags:* `organization`

### Delete an organization

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - organization that is to be deleted

### Get an organization

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of the organization to get

### Edit an organization

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of the organization to edit

### List an organization's webhooks

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of the organization

### Create a hook

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of the organization

### Delete a hook

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of the organization
* `id` - _required_ - id of the hook to delete

### Get a hook

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of the organization
* `id` - _required_ - id of the hook to get

### Update a hook

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of the organization
* `id` - _required_ - id of the hook to update

### List an organization's members

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of the organization

### Remove a member from an organization

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of the organization
* `username` - _required_ - username of the user

### Check if a user is a member of an organization

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of the organization
* `username` - _required_ - username of the user

### List an organization's public members

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of the organization

### Conceal a user's membership

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of the organization
* `username` - _required_ - username of the user

### Check if a user is a public member of an organization

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of the organization
* `username` - _required_ - username of the user

### Publicize a user's membership

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of the organization
* `username` - _required_ - username of the user

### List an organization's repos

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of the organization

### List an organization's teams

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of the organization

### Create a team

*Tags:* `organization`

#### Input Parameters
* `org` - _required_ - name of the organization

### Migrate a remote git repository

*Tags:* `repository`

### Search for repositories

*Tags:* `repository`

#### Input Parameters
* `q` - _optional_ - keyword
* `uid` - _optional_ - search only for repos that the user with the given id owns or contributes to
* `page` - _optional_ - page number of results to return (1-based)
* `limit` - _optional_ - page size of results, maximum page size is 50
* `mode` - _optional_ - type of repository to search for. Supported values are "fork", "source", "mirror" and "collaborative"
* `exclusive` - _optional_ - if `uid` is given, search only for repos that the user owns
* `sort` - _optional_ - sort repos by attribute. Supported values are "alpha", "created", "updated", "size", and "id". Default is "alpha"
* `order` - _optional_ - sort order, either "asc" (ascending) or "desc" (descending). Default is "asc", ignored if "sort" is not specified.

### Delete a repository

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo to delete
* `repo` - _required_ - name of the repo to delete

### Get a repository

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Get an archive of a repository

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `archive` - _required_ - archive to download, consisting of a git reference and archive

### List a repository's branches

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Retrieve a specific branch from a repository

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `branch` - _required_ - branch to get

### List a repository's collaborators

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Delete a collaborator from a repository

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `collaborator` - _required_ - username of the collaborator to delete

### Check if a user is a collaborator of a repository

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `collaborator` - _required_ - username of the collaborator

### Add a collaborator to a repository

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `collaborator` - _required_ - username of the collaborator to add

### Get a commit's combined status, by branch/tag/commit reference

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `ref` - _required_ - name of branch/tag/commit

### Get the EditorConfig definitions of a file in a repository

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `filepath` - _required_ - filepath of file to get

### List a repository's forks

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Fork a repository

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo to fork
* `repo` - _required_ - name of the repo to fork

### Get a single commit from a repository

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `sha` - _required_ - the commit hash

### Get specified ref or filtered repository's refs

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Get specified ref or filtered repository's refs

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `ref` - _required_ - part or full name of the ref

### Gets the tree of a repository.

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `sha` - _required_ - sha of the commit
* `recursive` - _optional_ - show all directories and files
* `page` - _optional_ - page number; the 'truncated' field in the response will be true if there are still more items after this page, false if the last page
* `per_page` - _optional_ - number of items per page; default is 1000 or what is set in app.ini as DEFAULT_GIT_TREES_PER_PAGE

### List the hooks in a repository

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Create a hook

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Delete a hook in a repository

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the hook to delete

### Get a hook

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the hook to get

### Edit a hook in a repository

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - index of the hook

### Test a push webhook

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the hook to test

### List a repository's issues

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `state` - _optional_ - whether issue is open or closed
* `labels` - _optional_ - comma separated list of labels. Fetch only issues that have any of this labels. Non existent labels are discarded
* `page` - _optional_ - page number of requested issues
* `q` - _optional_ - search string

### Create an issue. If using deadline only the date will be taken into account, and time of day ignored.

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### List all comments in a repository

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `since` - _optional_ - if provided, only comments updated since the provided time are returned.

### Delete a comment

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of comment to delete

### Edit a comment

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the comment to edit

### List an issue's tracked times

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - index of the issue

### Add a tracked time to a issue

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - index of the issue to add tracked time to

### Get an issue

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - index of the issue to get

### Edit an issue. If using deadline only the date will be taken into account, and time of day ignored.

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - index of the issue to edit

### List all comments on an issue

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - index of the issue
* `since` - _optional_ - if provided, only comments updated since the specified time are returned.

### Add a comment to an issue

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - index of the issue

### Delete a comment

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - this parameter is ignored
* `id` - _required_ - id of comment to delete

### Edit a comment

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - this parameter is ignored
* `id` - _required_ - id of the comment to edit

### Set an issue deadline. If set to null, the deadline is deleted. If using deadline only the date will be taken into account, and time of day ignored.

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - index of the issue to create or update a deadline on

### Remove all labels from an issue

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - index of the issue

### Get an issue's labels

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - index of the issue

### Add a label to an issue

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - index of the issue

### Replace an issue's labels

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - index of the issue

### Remove a label from an issue

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - index of the issue
* `id` - _required_ - id of the label to remove

### Start stopwatch on an issue.

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - index of the issue to create the stopwatch on

### Stop an issue's existing stopwatch.

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - index of the issue to stop the stopwatch on

### List a repository's keys

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `key_id` - _optional_ - the key_id to search for
* `fingerprint` - _optional_ - fingerprint of the key

### Add a key to a repository

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Delete a key from a repository

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the key to delete

### Get a repository's key by id

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the key to get

### Get all of a repository's labels

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Create a label

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Delete a label

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the label to delete

### Get a single label

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the label to get

### Update a label

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the label to edit

### Get all of a repository's opened milestones

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Create a milestone

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Delete a milestone

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the milestone to delete

### Get a milestone

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the milestone

### Update a milestone

*Tags:* `issue`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the milestone

### Sync a mirrored repository

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo to sync
* `repo` - _required_ - name of the repo to sync

### List a repo's pull requests

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `page` - _optional_ - Page number
* `state` - _optional_ - State of pull request: open or closed (optional)
    Possible values: closed, open, all.
* `sort` - _optional_ - Type of sort
    Possible values: oldest, recentupdate, leastupdate, mostcomment, leastcomment, priority.
* `milestone` - _optional_ - ID of the milestone
* `labels` - _optional_ - Label IDs

### Create a pull request

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Get a pull request

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - index of the pull request to get

### Update a pull request

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - index of the pull request to edit

### Check if a pull request has been merged

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - index of the pull request

### Merge a pull request

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `index` - _required_ - index of the pull request to merge

### Get a file from a repository

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `filepath` - _required_ - filepath of the file to get

### List a repo's releases

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `page` - _optional_ - page wants to load
* `per_page` - _optional_ - items count every page wants to load

### Create a release

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Delete a release

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the release to delete

### Get a release

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the release to get

### Update a release

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the release to edit

### List release's attachments

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the release

### Create a release attachment

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the release
* `name` - _optional_ - name of the attachment

### Delete a release attachment

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the release
* `attachment_id` - _required_ - id of the attachment to delete

### Get a release attachment

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the release
* `attachment_id` - _required_ - id of the attachment to get

### Edit a release attachment

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `id` - _required_ - id of the release
* `attachment_id` - _required_ - id of the attachment to edit

### List a repo's stargazers

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Get a commit's statuses

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `sha` - _required_ - sha of the commit

### Create a commit status

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `sha` - _required_ - sha of the commit

### List a repo's watchers

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Unwatch a repo

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Check if the current user is watching a repo

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Watch a repo

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### List a repository's tags

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### List a repo's tracked times

*Tags:* `repository`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### List a user's tracked times in a repo

*Tags:* `user`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo
* `user` - _required_ - username of user

### Get a repository by id

*Tags:* `repository`

#### Input Parameters
* `id` - _required_ - id of the repo to get

### Delete a team

*Tags:* `organization`

#### Input Parameters
* `id` - _required_ - id of the team to delete

### Get a team

*Tags:* `organization`

#### Input Parameters
* `id` - _required_ - id of the team to get

### Edit a team

*Tags:* `organization`

#### Input Parameters
* `id` - _required_ - id of the team to edit

### List a team's members

*Tags:* `organization`

#### Input Parameters
* `id` - _required_ - id of the team

### Remove a team member

*Tags:* `organization`

#### Input Parameters
* `id` - _required_ - id of the team
* `username` - _required_ - username of the user to remove

### List a particular member of team

*Tags:* `organization`

#### Input Parameters
* `id` - _required_ - id of the team
* `username` - _required_ - username of the member to list

### Add a team member

*Tags:* `organization`

#### Input Parameters
* `id` - _required_ - id of the team
* `username` - _required_ - username of the user to add

### List a team's repos

*Tags:* `organization`

#### Input Parameters
* `id` - _required_ - id of the team

### Remove a repository from a team

> This does not delete the repository, it only removes the repository from the team.

*Tags:* `organization`

#### Input Parameters
* `id` - _required_ - id of the team
* `org` - _required_ - organization that owns the repo to remove
* `repo` - _required_ - name of the repo to remove

### Add a repository to a team

*Tags:* `organization`

#### Input Parameters
* `id` - _required_ - id of the team
* `org` - _required_ - organization that owns the repo to add
* `repo` - _required_ - name of the repo to add

### search topics via keyword

*Tags:* `repository`

#### Input Parameters
* `q` - _required_ - keywords to search

### Get the authenticated user

*Tags:* `user`

### Delete email addresses

*Tags:* `user`

### List the authenticated user's email addresses

*Tags:* `user`

### Add email addresses

*Tags:* `user`

### List the authenticated user's followers

*Tags:* `user`

### List the users that the authenticated user is following

*Tags:* `user`

### Unfollow a user

*Tags:* `user`

#### Input Parameters
* `username` - _required_ - username of user to unfollow

### Check whether a user is followed by the authenticated user

*Tags:* `user`

#### Input Parameters
* `username` - _required_ - username of followed user

### Follow a user

*Tags:* `user`

#### Input Parameters
* `username` - _required_ - username of user to follow

### List the authenticated user's GPG keys

*Tags:* `user`

### Create a GPG key

*Tags:* `user`

### Remove a GPG key

*Tags:* `user`

#### Input Parameters
* `id` - _required_ - id of key to delete

### Get a GPG key

*Tags:* `user`

#### Input Parameters
* `id` - _required_ - id of key to get

### List the authenticated user's public keys

*Tags:* `user`

#### Input Parameters
* `fingerprint` - _optional_ - fingerprint of the key

### Create a public key

*Tags:* `user`

### Delete a public key

*Tags:* `user`

#### Input Parameters
* `id` - _required_ - id of key to delete

### Get a public key

*Tags:* `user`

#### Input Parameters
* `id` - _required_ - id of key to get

### List the current user's organizations

*Tags:* `organization`

### List the repos that the authenticated user owns or has access to

*Tags:* `user`

### Create a repository

*Tags:* `repository` `user`

### The repos that the authenticated user has starred

*Tags:* `user`

### Unstar the given repo

*Tags:* `user`

#### Input Parameters
* `owner` - _required_ - owner of the repo to unstar
* `repo` - _required_ - name of the repo to unstar

### Whether the authenticated is starring the repo

*Tags:* `user`

#### Input Parameters
* `owner` - _required_ - owner of the repo
* `repo` - _required_ - name of the repo

### Star the given repo

*Tags:* `user`

#### Input Parameters
* `owner` - _required_ - owner of the repo to star
* `repo` - _required_ - name of the repo to star

### List repositories watched by the authenticated user

*Tags:* `user`

### List all the teams a user belongs to

*Tags:* `user`

### List the current user's tracked times

*Tags:* `user`

### Search for users

*Tags:* `user`

#### Input Parameters
* `q` - _optional_ - keyword
* `uid` - _optional_ - ID of the user to search for
* `limit` - _optional_ - maximum number of users to return

### Check if one user is following another user

*Tags:* `user`

#### Input Parameters
* `follower` - _required_ - username of following user
* `followee` - _required_ - username of followed user

### Get a user

*Tags:* `user`

#### Input Parameters
* `username` - _required_ - username of user to get

### List the given user's followers

*Tags:* `user`

#### Input Parameters
* `username` - _required_ - username of user

### List the users that the given user is following

*Tags:* `user`

#### Input Parameters
* `username` - _required_ - username of user

### List the given user's GPG keys

*Tags:* `user`

#### Input Parameters
* `username` - _required_ - username of user

### Get a user's heatmap

*Tags:* `user`

#### Input Parameters
* `username` - _required_ - username of user to get

### List the given user's public keys

*Tags:* `user`

#### Input Parameters
* `username` - _required_ - username of user
* `fingerprint` - _optional_ - fingerprint of the key

### List a user's organizations

*Tags:* `organization`

#### Input Parameters
* `username` - _required_ - username of user

### List the repos owned by the given user

*Tags:* `user`

#### Input Parameters
* `username` - _required_ - username of user

### The repos that the given user has starred

*Tags:* `user`

#### Input Parameters
* `username` - _required_ - username of user

### List the repositories watched by a user

*Tags:* `user`

#### Input Parameters
* `username` - _required_ - username of the user

### List the authenticated user's access tokens

*Tags:* `user`

#### Input Parameters
* `username` - _required_ - username of user

### Create an access token

*Tags:* `user`

#### Input Parameters
* `username` - _required_ - username of user

### delete an access token

*Tags:* `user`

#### Input Parameters
* `username` - _required_ - username of user
* `token` - _required_ - token to be deleted

### Returns the version of the Gitea application

*Tags:* `miscellaneous`

## License

**flow**ground :- Telekom iPaaS / gitea-io-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
