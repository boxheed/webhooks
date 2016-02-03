# webhooks

Testing webhooks.

Editing this file in the GitHub UI does result in a webhook message.

Changed the header mapping to get the X- headers mapped through

Refactored the packages.

Added in routing on the user agent header for GitHub web hook

Routing didn't work on a wild carded header value.



## headers

```
content-length=5846, 
http_requestMethod=POST, 
x-github-event=push, 
x-github-delivery=3f381c00-ca7e-11e5-8fbe-17989828c7be, 
host=localhost:8080, 
http_requestUrl=http://localhost:8080/hooks/git, 
connection=close, 
id=98ccf1a6-34f1-4c78-2cc3-ca5baa072587, 
contentType=application/json;charset=UTF-8, 
accept=*/*, 
user-agent=GitHub-Hookshot/21f57ba, 
timestamp=1454507929898
```

## Payload
```
{
   compare=https://github.com/boxheed/webhooks/compare/ba83770642d9...afb29bd64054,
   head_commit=   {
      id=afb29bd640540cb1ef96bc5b9d0b7cc961778d39,
      distinct=true,
      message=Commit 2,
      timestamp=2016-02-03T10:28:19      Z,
      url=https://github.com/boxheed/webhooks/commit/afb29bd640540cb1ef96bc5b9d0b7cc961778d39,
      author=      {
         name=Andrew Dunn,
         email=adunn@mango-solutions.com
      },
      committer=      {
         name=Andrew Dunn,
         email=adunn@mango-solutions.com
      },
      added=      [

      ],
      removed=      [

      ],
      modified=      [
         README.md
      ]
   },
   pusher=   {
      name=boxheed,
      email=boxheed@users.noreply.github.com
   },
   before=ba83770642d96a551ff18157a537cc7290ed8aa8,
   created=false,
   forced=false,
   base_ref=null,
   repository=   {
      id=50917788,
      name=webhooks,
      full_name=boxheed/webhooks,
      owner=      {
         name=boxheed,
         email=boxheed@users.noreply.github.com
      },
      private=false,
      html_url=https://github.com/boxheed/webhooks,
      description=,
      fork=false,
      url=https://github.com/boxheed/webhooks,
      forks_url=https://api.github.com/repos/boxheed/webhooks/forks,
      keys_url=https://api.github.com/repos/boxheed/webhooks/keys      {
         /key_id
      },
      collaborators_url=https://api.github.com/repos/boxheed/webhooks/collaborators      {
         /collaborator
      },
      teams_url=https://api.github.com/repos/boxheed/webhooks/teams,
      hooks_url=https://api.github.com/repos/boxheed/webhooks/hooks,
      issue_events_url=https://api.github.com/repos/boxheed/webhooks/issues/events      {
         /number
      },
      events_url=https://api.github.com/repos/boxheed/webhooks/events,
      assignees_url=https://api.github.com/repos/boxheed/webhooks/assignees      {
         /user
      },
      branches_url=https://api.github.com/repos/boxheed/webhooks/branches      {
         /branch
      },
      tags_url=https://api.github.com/repos/boxheed/webhooks/tags,
      blobs_url=https://api.github.com/repos/boxheed/webhooks/git/blobs      {
         /sha
      },
      git_tags_url=https://api.github.com/repos/boxheed/webhooks/git/tags      {
         /sha
      },
      git_refs_url=https://api.github.com/repos/boxheed/webhooks/git/refs      {
         /sha
      },
      trees_url=https://api.   github.com/repos/boxheed/webhooks/git/trees      {
         /sha
      },
      statuses_url=https://api.github.com/repos/boxheed/webhooks/statuses/      {
         sha
      },
      languages_url=https://api.github.com/repos/boxheed/webhooks/languages,
      stargazers_url=https://api.github.com/repos/boxheed/webhooks/stargazers,
      contributors_url=https://api.github.com/repos/boxheed/webhooks/contributors,
      subscribers_url=https://api.github.com/repos/boxheed/webhooks/subscribers,
      subscription_url=https://api.github.com/repos/boxheed/webhooks/subscription,
      commits_url=https://api.github.com/repos/boxheed/webhooks/commits      {
         /sha
      },
      git_commits_url=https://api.github.com/repos/boxheed/webhooks/git/commits      {
         /sha
      },
      comments_url=https://api.github.com/repos/boxheed/webhooks/comments      {
         /number
      },
      issue_comment_url=https://api.github.com/repos/boxheed/webhooks/issues/comments      {
         /number
      },
      contents_url=https://api.github.com/repos/boxheed/webhooks/contents/      {
         +path
      },
      compare_url=https://api.github.com/repos/boxheed/webhooks/compare/      {
         base
      }      ...      {
         head
      },
      merges_url=https://api.github.com/repos/boxheed/webhooks/merges,
      archive_url=https://api.github.com/repos/boxheed/webhooks/      {
         archive_format
      }      {
         /ref
      },
      downloads_url=https://api.github.com/repos/boxheed/webhooks/downloads,
      issues_url=https://api.github.com/repos/boxheed/webhooks/issues      {
         /number
      },
      pulls_url=https://api.github.com/repos/boxheed/webhooks/pulls      {
         /number
      },
      milestones_url=https://api.github.com/repos/boxheed/webhooks/milestones      {
         /number
      },
      notifications_url=https://api.github.com/repos/boxheed/webhooks/notifications      {
         ?since,
         all,
         participating
      },
      labels_url=https://api.github.com/repos/boxheed/webhooks/labels      {
         /name
      },
      releases_url=https://api.github.com/repos/boxheed/webhooks/releases      {
         /id
      },
      deployments_url=https://api.github.com/repos/boxheed/webhooks/deployments,
      created_at=1454414691,
      updated_at=2016-02-02T12:04:51      Z,
      pushed_at=1454495304,
      git_url=git://github.com/boxheed/webhooks.git,
      ssh_url=git@github.com:boxheed/webhooks.git,
      clone_url=https://github.com/boxheed/webhooks.git,
      svn_url=https://github.com/boxheed/webhooks,
      homepage=null,
      size=7,
      starga                                        zers_count=0,
      watchers_count=0,
      language=null,
      has_issues=true,
      has_downloads=true,
      has_wiki=true,
      has_pages=false,
      forks_count=0,
      mirror_url=null,
      open_issues_count=0,
      forks=0,
      open_issues=0,
      watchers=0,
      default_branch=master,
      stargazers=0,
      master_branch=master
   },
   ref=refs/heads/master,
   deleted=false,
   sender=   {
      login=boxheed,
      id=7342194,
      avatar_url=https://avatars.githubusercontent.com/u/7342194?v=3,
      gravatar_id=,
      url=https://api.github.com/users/boxheed,
      html_url=https://github.com/boxheed,
      followers_url=https://api.github.com/users/boxheed/followers,
      following_url=https://api.github.com/users/boxheed/following      {
         /other_user
      },
      gists_url=https://api.github.com/users/boxheed/gists      {
         /gist_id
      },
      starred_url=https://api.github.com/users/boxheed/starred      {
         /owner
      }      {
         /repo
      },
      subscriptions_url=https://api.github.com/users/boxheed/subscriptions,
      organizations_url=https://api.github.com/users/boxheed/orgs,
      repos_url=https://api.github.com/users/boxheed/repos,
      events_url=https://api.github.com/users/boxheed/events      {
         /privacy
      },
      received_events_url=https://api.github.com/users/boxheed/received_events,
      type=User,
      site_admin=false
   },
   commits=   [
      {
         id=d4ae696296de9b3619b1954234d9c588c7f66f6a,
         distinct=true,
         message=Commit 1,
         timestamp=2016-02-03T10:28:03         Z,
         url=https://github.com/boxheed/webhooks/commit/d4ae696296de9b3619b1954234d9c588c7f66f6a,
         author=         {
            name=Andrew Dunn,
            email=adunn@mango-solutions.com
         },
         committer=         {
            name=Andrew Dunn,
            email=adunn@mango-solutions.com
         },
         added=         [

         ],
         removed=         [

         ],
         modified=         [
            README.md
         ]
      },
      {
         id=afb29bd640540cb1ef96bc5b9d0b7cc961778d39,
         distinct=true,
         message=Commit 2,
         timestamp=2016-02-03T10:28:19         Z,
         url=https://github.com/boxheed/webhooks/commit/afb29bd640540cb1ef96bc5b9d0b7cc961778d39,
         author=         {
            name=Andrew Dunn,
            email=adunn@mango-solutions.com
         },
         committer=         {
            name=Andrew Dunn,
            email=adunn@mango-solutions.com
         },
         added=         [

         ],
         removed=         [

         ],
         modified=         [
            README.md
         ]
      }
   ],
   after=afb29bd640540cb1ef96bc5b9d0b7cc961778d39
}         
```



routing again....

picking the x-github-event header for github requests.
