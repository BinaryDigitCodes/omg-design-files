// Weblog Configuration

;; About your weblog
;; -----------------

Weblog title: B's Cafe ☕
Weblog description: Welcome to my cozy space where I share favorite nerdy things while sipping my daily cup of coffee ☕
Author: BinaryDigit
Canonical domain: binarydigit.cafe

;; General config stuff
;; --------------------

Separator:  · 
// Navigation: about, another-page, <a href="https://example.com">Example</a>, [Example](https://example.com)


;; Time stuff
;; ----------

; You can use a timezone value from the "TZ database name" column on this 
; web page: https://en.wikipedia.org/wiki/List_of_tz_database_time_zones

Timezone: America/New_York
Date format: M j, Y

;; Feeds
;; -----

Feed post count: 10

;; Posts
;; -----

Post path format: /

Default post: <<[---
Date: $date
Tags: 
---

# New Title

]>>


;; Recent posts {recent-posts}
;; ---------------------------

Recent posts count: 5
Recent posts format: <<[
<ul>
[post:begin]<li><a href="$location">$title</a></li>[post:end]
</ul>]>>


;; Post list {post-list}
;; ---------------------

Post list format: <<[
<ul>
[post:begin]<li><a href="$location">$title</a></li>[post:end]
</ul>]>>


;; Search
;; ------

Search status: enabled
Search results success message: There [is|are] $count [result|results] for your search:
Search results failure message: There were no results found for your search.
Search results format: <<[
<h2>Results for “$search”</h2>
<p>$search_results_message</p>
[post:begin]<h3><a href="$location">$title</a></h3>
<p>$date</p>
<p>$snippet</p>[post:end]
]>>


;; Tags {tags}
;; -----------

Tag path: /tag/
Tags format: <<[
[tag:begin]<a class="tag" href="$tag_location">$tag</a>[tag:end]
]>>
