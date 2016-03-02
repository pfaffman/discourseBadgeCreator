# discourseBadgeCreator
Python script to create sets of badges in Discourse.

Jay Pfaffman <jay@pfaffman.com>
License: GPL

## How it Works:

Stick these files in a folder, edit discourseBadgeCreator.yml to have
your API key and your username (from /admin/api).

See discourseBadgeCreator.yml for defaults.

usage: discourseBadgeCreator [-h] [--group GROUP] [--enabled ENABLED]
                             [--groupID GROUPID] [--multiple MULTIPLE]
                             [--asTitle ASTITLE] [--listable LISTABLE]
                             [--revoke REVOKE] [--showPosts SHOWPOSTS]
                             [--goldLikes GOLDLIKES] [-v V]
                             title icon tag

For example, 

    ./discourseBadgeCreator "Cool Badge" fa-anchor sometag
	
creates three badges

- Bronze: user posted in CATEGORY (defined in discourseBadgeCreator.yml)
with tag "sometag".

- Silver: user posted sometag in CATEGORY and someone from GROUP
  (defined in config file) liked it.
  
- Gold: user posted sometag in CATEGORY and someone from GROUP
  (defined in config file) liked it, and has at least GOLDLIKES likes
  
  
