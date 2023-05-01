# Comparing `tmp/twitter_api_py-0.1.0.tar.gz` & `tmp/twitter_api_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter_api_py-0.1.0.tar", max compression
+gzip compressed data, was "twitter_api_py-0.2.0.tar", max compression
```

## Comparing `twitter_api_py-0.1.0.tar` & `twitter_api_py-0.2.0.tar`

### file list

```diff
@@ -1,205 +1,218 @@
--rw-r--r--   0        0        0     1957 2023-04-23 12:48:05.383339 twitter_api_py-0.1.0/README.md
--rw-r--r--   0        0        0     1430 2023-04-23 12:43:18.589780 twitter_api_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      180 2023-04-22 10:21:01.801508 twitter_api_py-0.1.0/twitter_api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:09.975602 twitter_api_py-0.1.0/twitter_api/api/__init__.py
--rw-r--r--   0        0        0      281 2023-04-22 04:51:08.637342 twitter_api_py-0.1.0/twitter_api/api/resources/api_resources.py
--rw-r--r--   0        0        0      437 2023-04-22 10:21:01.801508 twitter_api_py-0.1.0/twitter_api/api/resources/oauth2_invalidate_token/__init__.py
--rw-r--r--   0        0        0     2371 2023-04-22 10:21:01.801508 twitter_api_py-0.1.0/twitter_api/api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py
--rw-r--r--   0        0        0      332 2023-04-22 10:21:01.801508 twitter_api_py-0.1.0/twitter_api/api/resources/oauth2_token/__init__.py
--rw-r--r--   0        0        0     2186 2023-04-22 10:21:01.801508 twitter_api_py-0.1.0/twitter_api/api/resources/oauth2_token/post_oauth2_token.py
--rw-r--r--   0        0        0      541 2023-04-22 10:21:01.801508 twitter_api_py-0.1.0/twitter_api/api/resources/v2_dm_conversation_messages/__init__.py
--rw-r--r--   0        0        0     2331 2023-04-22 13:57:13.753532 twitter_api_py-0.1.0/twitter_api/api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py
--rw-r--r--   0        0        0      441 2023-04-22 10:21:01.801508 twitter_api_py-0.1.0/twitter_api/api/resources/v2_dm_conversations/__init__.py
--rw-r--r--   0        0        0     2271 2023-04-22 13:57:13.753532 twitter_api_py-0.1.0/twitter_api/api/resources/v2_dm_conversations/post_v2_dm_conversations.py
--rw-r--r--   0        0        0      664 2023-04-22 10:21:01.801508 twitter_api_py-0.1.0/twitter_api/api/resources/v2_dm_conversations_with_messages/__init__.py
--rw-r--r--   0        0        0     2405 2023-04-22 13:57:13.463531 twitter_api_py-0.1.0/twitter_api/api/resources/v2_dm_conversations_with_messages/post_v2_dm_conversations_with_messages.py
--rw-r--r--   0        0        0      429 2023-04-22 10:21:01.801508 twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweet/__init__.py
--rw-r--r--   0        0        0     1445 2023-04-22 13:57:13.353530 twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweet/delete_v2_tweet.py
--rw-r--r--   0        0        0     3101 2023-04-22 13:57:13.463531 twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweet/get_v2_tweet.py
--rw-r--r--   0        0        0      458 2023-04-22 10:21:01.801508 twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweet_retweeted_by/__init__.py
--rw-r--r--   0        0        0     6221 2023-04-23 02:38:02.711525 twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py
--rw-r--r--   0        0        0      428 2023-04-22 10:21:01.801508 twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets/__init__.py
--rw-r--r--   0        0        0     2990 2023-04-22 14:21:22.792136 twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets/get_v2_tweets.py
--rw-r--r--   0        0        0     2949 2023-04-22 13:57:13.193529 twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets/post_v2_tweets.py
--rw-r--r--   0        0        0      438 2023-04-22 10:21:01.801508 twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets_search_all/__init__.py
--rw-r--r--   0        0        0     5760 2023-04-23 02:38:07.121389 twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py
--rw-r--r--   0        0        0      471 2023-04-22 10:21:01.801508 twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets_search_recent/__init__.py
--rw-r--r--   0        0        0     5859 2023-04-23 02:41:02.315961 twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py
--rw-r--r--   0        0        0      471 2023-04-22 10:21:01.801508 twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets_search_stream/__init__.py
--rw-r--r--   0        0        0     5265 2023-04-23 02:41:29.315129 twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py
--rw-r--r--   0        0        0      770 2023-04-22 10:21:01.801508 twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets_search_stream_rules/__init__.py
--rw-r--r--   0        0        0     2118 2023-04-22 13:57:13.193529 twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py
--rw-r--r--   0        0        0     3094 2023-04-22 13:57:13.063528 twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py
--rw-r--r--   0        0        0      275 2023-04-22 10:21:01.801508 twitter_api_py-0.1.0/twitter_api/api/resources/v2_user/__init__.py
--rw-r--r--   0        0        0     2789 2023-04-22 13:57:12.943528 twitter_api_py-0.1.0/twitter_api/api/resources/v2_user/get_v2_user.py
--rw-r--r--   0        0        0      371 2023-04-22 10:21:01.801508 twitter_api_py-0.1.0/twitter_api/api/resources/v2_user_followers/__init__.py
--rw-r--r--   0        0        0     6174 2023-04-23 02:41:58.774221 twitter_api_py-0.1.0/twitter_api/api/resources/v2_user_followers/get_v2_user_followers.py
--rw-r--r--   0        0        0      376 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/api/resources/v2_user_following/__init__.py
--rw-r--r--   0        0        0     1916 2023-04-22 13:57:13.753532 twitter_api_py-0.1.0/twitter_api/api/resources/v2_user_following/post_v2_user_following.py
--rw-r--r--   0        0        0      391 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/api/resources/v2_user_liked_tweets/__init__.py
--rw-r--r--   0        0        0     7619 2023-04-23 02:42:30.723235 twitter_api_py-0.1.0/twitter_api/api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py
--rw-r--r--   0        0        0      367 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/api/resources/v2_user_retweets/__init__.py
--rw-r--r--   0        0        0     1922 2023-04-22 13:57:12.743526 twitter_api_py-0.1.0/twitter_api/api/resources/v2_user_retweets/post_v2_user_retweets.py
--rw-r--r--   0        0        0      331 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/api/resources/v2_user_tweets/__init__.py
--rw-r--r--   0        0        0     8034 2023-04-23 02:43:00.032330 twitter_api_py-0.1.0/twitter_api/api/resources/v2_user_tweets/get_v2_user_tweets.py
--rw-r--r--   0        0        0      279 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/api/resources/v2_users/__init__.py
--rw-r--r--   0        0        0     2689 2023-04-22 13:57:12.793527 twitter_api_py-0.1.0/twitter_api/api/resources/v2_users/get_v2_users.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:10.025603 twitter_api_py-0.1.0/twitter_api/api/types/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 17:04:18.882718 twitter_api_py-0.1.0/twitter_api/api/types/oauth1/__init__.py
--rw-r--r--   0        0        0      742 2023-04-16 09:10:49.011162 twitter_api_py-0.1.0/twitter_api/api/types/oauth1/oauth1_access_token.py
--rw-r--r--   0        0        0     2688 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/api/types/oauth1/oauth1_authorization.py
--rw-r--r--   0        0        0        0 2023-04-09 09:46:11.323030 twitter_api_py-0.1.0/twitter_api/api/types/oauth2/__init__.py
--rw-r--r--   0        0        0      667 2023-04-16 12:02:08.887550 twitter_api_py-0.1.0/twitter_api/api/types/oauth2/oauth2_access_token.py
--rw-r--r--   0        0        0     2718 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/api/types/oauth2/oauth2_authorization.py
--rw-r--r--   0        0        0       55 2023-04-02 02:22:08.622273 twitter_api_py-0.1.0/twitter_api/api/types/v2_cashtag.py
--rw-r--r--   0        0        0        0 2023-04-04 00:14:28.746398 twitter_api_py-0.1.0/twitter_api/api/types/v2_dm_conversation/__init__.py
--rw-r--r--   0        0        0      345 2023-04-09 09:46:44.353033 twitter_api_py-0.1.0/twitter_api/api/types/v2_dm_conversation/dm_conversation.py
--rw-r--r--   0        0        0      205 2023-04-04 14:28:03.516388 twitter_api_py-0.1.0/twitter_api/api/types/v2_dm_conversation/dm_conversation_attachment.py
--rw-r--r--   0        0        0       64 2023-04-04 00:15:15.770562 twitter_api_py-0.1.0/twitter_api/api/types/v2_dm_conversation/dm_conversation_id.py
--rw-r--r--   0        0        0      598 2023-04-05 12:42:42.545017 twitter_api_py-0.1.0/twitter_api/api/types/v2_dm_conversation/dm_conversation_message.py
--rw-r--r--   0        0        0        0 2023-04-04 00:15:59.434445 twitter_api_py-0.1.0/twitter_api/api/types/v2_dm_event/__init__.py
--rw-r--r--   0        0        0       57 2023-04-04 00:16:14.175754 twitter_api_py-0.1.0/twitter_api/api/types/v2_dm_event/dm_event_id.py
--rw-r--r--   0        0        0      293 2023-04-15 05:02:40.690195 twitter_api_py-0.1.0/twitter_api/api/types/v2_domain.py
--rw-r--r--   0        0        0      226 2023-04-03 14:33:02.144299 twitter_api_py-0.1.0/twitter_api/api/types/v2_entity.py
--rw-r--r--   0        0        0      616 2023-04-15 16:16:36.758131 twitter_api_py-0.1.0/twitter_api/api/types/v2_expansion.py
--rw-r--r--   0        0        0        0 2023-04-15 05:54:42.060789 twitter_api_py-0.1.0/twitter_api/api/types/v2_geo/__init__.py
--rw-r--r--   0        0        0      209 2023-04-15 05:55:44.170800 twitter_api_py-0.1.0/twitter_api/api/types/v2_geo/geo.py
--rw-r--r--   0        0        0       55 2023-04-02 02:15:19.761414 twitter_api_py-0.1.0/twitter_api/api/types/v2_hashtag.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:10.035603 twitter_api_py-0.1.0/twitter_api/api/types/v2_media/__init__.py
--rw-r--r--   0        0        0     1389 2023-04-15 06:07:09.620870 twitter_api_py-0.1.0/twitter_api/api/types/v2_media/media.py
--rw-r--r--   0        0        0      570 2023-04-15 15:58:56.812733 twitter_api_py-0.1.0/twitter_api/api/types/v2_media/media_field.py
--rw-r--r--   0        0        0      100 2023-04-01 16:14:08.728923 twitter_api_py-0.1.0/twitter_api/api/types/v2_media/media_id.py
--rw-r--r--   0        0        0       56 2023-04-01 09:17:10.035603 twitter_api_py-0.1.0/twitter_api/api/types/v2_media/media_key.py
--rw-r--r--   0        0        0      376 2023-04-15 06:00:40.800828 twitter_api_py-0.1.0/twitter_api/api/types/v2_media/media_non_public_metrics.py
--rw-r--r--   0        0        0      411 2023-04-15 06:02:11.910834 twitter_api_py-0.1.0/twitter_api/api/types/v2_media/media_organic_metrics.py
--rw-r--r--   0        0        0      412 2023-04-15 06:03:23.150843 twitter_api_py-0.1.0/twitter_api/api/types/v2_media/media_promoted_metrics.py
--rw-r--r--   0        0        0      190 2023-04-15 06:04:09.220847 twitter_api_py-0.1.0/twitter_api/api/types/v2_media/media_public_metrics.py
--rw-r--r--   0        0        0      211 2023-04-15 06:06:05.030862 twitter_api_py-0.1.0/twitter_api/api/types/v2_media/media_variants.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:10.035603 twitter_api_py-0.1.0/twitter_api/api/types/v2_place/__init__.py
--rw-r--r--   0        0        0      643 2023-04-15 05:56:35.000801 twitter_api_py-0.1.0/twitter_api/api/types/v2_place/place.py
--rw-r--r--   0        0        0      348 2023-04-15 15:58:30.892600 twitter_api_py-0.1.0/twitter_api/api/types/v2_place/place_field.py
--rw-r--r--   0        0        0       94 2023-04-01 09:17:10.045603 twitter_api_py-0.1.0/twitter_api/api/types/v2_place/place_id.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:10.045603 twitter_api_py-0.1.0/twitter_api/api/types/v2_poll/__init__.py
--rw-r--r--   0        0        0      601 2023-04-15 06:10:52.180889 twitter_api_py-0.1.0/twitter_api/api/types/v2_poll/poll.py
--rw-r--r--   0        0        0      272 2023-04-15 15:58:36.582629 twitter_api_py-0.1.0/twitter_api/api/types/v2_poll/poll_field.py
--rw-r--r--   0        0        0       54 2023-04-01 09:17:10.045603 twitter_api_py-0.1.0/twitter_api/api/types/v2_poll/poll_id.py
--rw-r--r--   0        0        0      164 2023-04-15 06:09:28.320883 twitter_api_py-0.1.0/twitter_api/api/types/v2_poll/poll_option.py
--rw-r--r--   0        0        0        0 2023-04-02 02:04:07.967716 twitter_api_py-0.1.0/twitter_api/api/types/v2_retweet/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-04 14:56:44.417296 twitter_api_py-0.1.0/twitter_api/api/types/v2_retweet/retweet.py
--rw-r--r--   0        0        0      400 2023-04-04 14:28:04.506389 twitter_api_py-0.1.0/twitter_api/api/types/v2_retweet/retweet_entities.py
--rw-r--r--   0        0        0      929 2023-04-04 14:28:04.676389 twitter_api_py-0.1.0/twitter_api/api/types/v2_retweet/retweet_entities_description.py
--rw-r--r--   0        0        0      241 2023-04-04 14:28:03.836388 twitter_api_py-0.1.0/twitter_api/api/types/v2_retweet/retweet_entities_description_cashtag.py
--rw-r--r--   0        0        0      241 2023-04-04 14:56:33.177292 twitter_api_py-0.1.0/twitter_api/api/types/v2_retweet/retweet_entities_description_hashtag.py
--rw-r--r--   0        0        0      250 2023-04-04 14:57:14.027308 twitter_api_py-0.1.0/twitter_api/api/types/v2_retweet/retweet_entities_description_mention.py
--rw-r--r--   0        0        0      258 2023-04-02 02:13:19.847028 twitter_api_py-0.1.0/twitter_api/api/types/v2_retweet/retweet_entities_description_url.py
--rw-r--r--   0        0        0      338 2023-04-02 02:10:33.754809 twitter_api_py-0.1.0/twitter_api/api/types/v2_retweet/retweet_entities_url.py
--rw-r--r--   0        0        0      258 2023-04-10 15:48:58.984612 twitter_api_py-0.1.0/twitter_api/api/types/v2_retweet/retweet_includes.py
--rw-r--r--   0        0        0      219 2023-04-02 02:26:55.269961 twitter_api_py-0.1.0/twitter_api/api/types/v2_retweet/retweet_public_metrics.py
--rw-r--r--   0        0        0      352 2023-04-02 02:04:56.864520 twitter_api_py-0.1.0/twitter_api/api/types/v2_retweet/retweet_withheld.py
--rw-r--r--   0        0        0        0 2023-04-09 09:46:44.373033 twitter_api_py-0.1.0/twitter_api/api/types/v2_rule/__init__.py
--rw-r--r--   0        0        0      319 2023-04-09 09:46:44.433033 twitter_api_py-0.1.0/twitter_api/api/types/v2_rule/rule.py
--rw-r--r--   0        0        0       54 2023-04-09 09:46:44.373033 twitter_api_py-0.1.0/twitter_api/api/types/v2_rule/rule_id.py
--rw-r--r--   0        0        0       55 2023-04-09 09:46:44.433033 twitter_api_py-0.1.0/twitter_api/api/types/v2_rule/rule_tag.py
--rw-r--r--   0        0        0     1411 2023-04-23 06:01:36.209583 twitter_api_py-0.1.0/twitter_api/api/types/v2_scope.py
--rw-r--r--   0        0        0      198 2023-04-14 15:29:17.871033 twitter_api_py-0.1.0/twitter_api/api/types/v2_search_query.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:10.045603 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/__init__.py
--rw-r--r--   0        0        0     6442 2023-04-18 13:43:34.885017 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet.py
--rw-r--r--   0        0        0      309 2023-04-04 14:19:50.365994 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_attachments.py
--rw-r--r--   0        0        0      229 2023-04-04 14:30:09.146468 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_context_annotation.py
--rw-r--r--   0        0        0      314 2023-04-01 09:17:36.515599 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_edit_controls.py
--rw-r--r--   0        0        0      720 2023-04-01 09:17:36.415599 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_entities.py
--rw-r--r--   0        0        0      333 2023-04-01 09:17:36.415599 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_entities_annotation.py
--rw-r--r--   0        0        0      247 2023-04-01 09:17:36.415599 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_entities_cashtag.py
--rw-r--r--   0        0        0      247 2023-04-01 09:17:36.415599 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_entities_hashtag.py
--rw-r--r--   0        0        0      317 2023-04-04 14:57:19.327310 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_entities_mention.py
--rw-r--r--   0        0        0      415 2023-04-15 03:52:45.757502 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_entities_url.py
--rw-r--r--   0        0        0     1910 2023-04-23 06:33:19.778673 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_field.py
--rw-r--r--   0        0        0      288 2023-04-01 09:17:36.415599 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_geo.py
--rw-r--r--   0        0        0      231 2023-04-01 09:17:37.035599 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_geo_coordinates.py
--rw-r--r--   0        0        0       59 2023-04-01 09:17:10.065603 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_id.py
--rw-r--r--   0        0        0      287 2023-04-01 09:17:37.035599 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_non_public_metrics.py
--rw-r--r--   0        0        0      285 2023-04-01 09:17:36.415599 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_organic_metrics.py
--rw-r--r--   0        0        0      286 2023-04-01 09:17:36.415599 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_promoted_metrics.py
--rw-r--r--   0        0        0      437 2023-04-09 15:28:28.034225 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_public_metrics.py
--rw-r--r--   0        0        0      256 2023-04-15 10:39:45.485596 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_referenced_tweet.py
--rw-r--r--   0        0        0     6880 2023-04-23 06:38:09.298573 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_response_body.py
--rw-r--r--   0        0        0      387 2023-04-02 01:59:57.044158 twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_withheld.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:10.065603 twitter_api_py-0.1.0/twitter_api/api/types/v2_user/__init__.py
--rw-r--r--   0        0        0      846 2023-04-04 14:57:25.117313 twitter_api_py-0.1.0/twitter_api/api/types/v2_user/user.py
--rw-r--r--   0        0        0      608 2023-04-15 16:00:19.963155 twitter_api_py-0.1.0/twitter_api/api/types/v2_user/user_field.py
--rw-r--r--   0        0        0       54 2023-04-01 09:17:10.065603 twitter_api_py-0.1.0/twitter_api/api/types/v2_user/user_id.py
--rw-r--r--   0        0        0      128 2023-04-02 07:41:55.232378 twitter_api_py-0.1.0/twitter_api/api/types/v2_user/username.py
--rw-r--r--   0        0        0       81 2023-04-01 09:17:10.075603 twitter_api_py-0.1.0/twitter_api/client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/client/oauth_flow/__init__.py
--rw-r--r--   0        0        0     2382 2023-04-23 04:09:09.615147 twitter_api_py-0.1.0/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py
--rw-r--r--   0        0        0     1139 2023-04-23 04:10:20.734739 twitter_api_py-0.1.0/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py
--rw-r--r--   0        0        0      626 2023-04-23 04:10:49.204576 twitter_api_py-0.1.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py
--rw-r--r--   0        0        0     2834 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py
--rw-r--r--   0        0        0      636 2023-04-22 10:25:05.195265 twitter_api_py-0.1.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py
--rw-r--r--   0        0        0        0 2023-04-09 09:46:11.283030 twitter_api_py-0.1.0/twitter_api/client/oauth_session/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/__init__.py
--rw-r--r--   0        0        0      263 2023-04-23 04:09:21.375079 twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/oauth1_access_token/__init__.py
--rw-r--r--   0        0        0      999 2023-04-23 04:09:09.705146 twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py
--rw-r--r--   0        0        0      355 2023-04-23 04:10:01.504850 twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/__init__.py
--rw-r--r--   0        0        0      707 2023-04-23 04:09:50.094915 twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py
--rw-r--r--   0        0        0      337 2023-04-23 04:10:33.544666 twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/oauth1_authorize/__init__.py
--rw-r--r--   0        0        0      621 2023-04-23 04:10:20.674740 twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py
--rw-r--r--   0        0        0      290 2023-04-23 04:11:05.304483 twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/oauth1_request_token/__init__.py
--rw-r--r--   0        0        0      672 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py
--rw-r--r--   0        0        0      406 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/oauth2_authorize/__init__.py
--rw-r--r--   0        0        0      657 2023-04-23 04:37:06.487761 twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py
--rw-r--r--   0        0        0      432 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/session_resources.py
--rw-r--r--   0        0        0      280 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/__init__.py
--rw-r--r--   0        0        0     1451 2023-04-23 04:36:42.767835 twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py
--rw-r--r--   0        0        0      658 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/client/oauth_session/twitter_oauth1_async_mock_session.py
--rw-r--r--   0        0        0     1824 2023-04-23 04:10:11.644791 twitter_api_py-0.1.0/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py
--rw-r--r--   0        0        0     3197 2023-04-23 04:10:49.184576 twitter_api_py-0.1.0/twitter_api/client/oauth_session/twitter_oauth1_real_session.py
--rw-r--r--   0        0        0     1790 2023-04-23 12:07:01.176960 twitter_api_py-0.1.0/twitter_api/client/oauth_session/twitter_oauth1_session.py
--rw-r--r--   0        0        0      458 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/client/oauth_session/twitter_oauth2_async_mock_session.py
--rw-r--r--   0        0        0     1490 2023-04-23 04:28:04.529740 twitter_api_py-0.1.0/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py
--rw-r--r--   0        0        0     2844 2023-04-23 04:28:04.509740 twitter_api_py-0.1.0/twitter_api/client/oauth_session/twitter_oauth2_real_session.py
--rw-r--r--   0        0        0     1316 2023-04-23 12:07:01.176960 twitter_api_py-0.1.0/twitter_api/client/oauth_session/twitter_oauth2_session.py
--rw-r--r--   0        0        0        0 2023-04-01 17:37:10.337565 twitter_api_py-0.1.0/twitter_api/client/request/__init__.py
--rw-r--r--   0        0        0     1512 2023-04-22 10:33:52.357373 twitter_api_py-0.1.0/twitter_api/client/request/request_async_client.py
--rw-r--r--   0        0        0      236 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/client/request/request_async_mock_client.py
--rw-r--r--   0        0        0     5046 2023-04-22 10:32:57.145053 twitter_api_py-0.1.0/twitter_api/client/request/request_async_real_client.py
--rw-r--r--   0        0        0     1771 2023-04-09 09:46:44.373033 twitter_api_py-0.1.0/twitter_api/client/request/request_client.py
--rw-r--r--   0        0        0     3312 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/client/request/request_mock_client.py
--rw-r--r--   0        0        0     6891 2023-04-22 10:28:00.052596 twitter_api_py-0.1.0/twitter_api/client/request/request_real_client.py
--rw-r--r--   0        0        0    16976 2023-04-22 10:53:13.689235 twitter_api_py-0.1.0/twitter_api/client/twitter_api_async_client.py
--rw-r--r--   0        0        0     3017 2023-04-22 10:48:54.401043 twitter_api_py-0.1.0/twitter_api/client/twitter_api_async_mock_client.py
--rw-r--r--   0        0        0     5274 2023-04-22 10:51:32.996050 twitter_api_py-0.1.0/twitter_api/client/twitter_api_async_real_client.py
--rw-r--r--   0        0        0    16309 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/client/twitter_api_client.py
--rw-r--r--   0        0        0    13750 2023-04-22 10:47:45.448862 twitter_api_py-0.1.0/twitter_api/client/twitter_api_mock_client.py
--rw-r--r--   0        0        0     4859 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/client/twitter_api_real_client.py
--rw-r--r--   0        0        0    10199 2023-04-15 06:29:11.890993 twitter_api_py-0.1.0/twitter_api/error.py
--rw-r--r--   0        0        0        0 2023-04-02 08:29:19.122099 twitter_api_py-0.1.0/twitter_api/rate_limit/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 08:53:21.142020 twitter_api_py-0.1.0/twitter_api/rate_limit/manager/__init__.py
--rw-r--r--   0        0        0     2311 2023-04-23 01:30:13.950504 twitter_api_py-0.1.0/twitter_api/rate_limit/manager/dict_rate_limit_manager.py
--rw-r--r--   0        0        0      525 2023-04-23 01:32:37.383610 twitter_api_py-0.1.0/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py
--rw-r--r--   0        0        0        0 2023-04-23 01:25:28.771650 twitter_api_py-0.1.0/twitter_api/rate_limit/manager/handlers/__init__.py
--rw-r--r--   0        0        0     1290 2023-04-23 04:23:32.250891 twitter_api_py-0.1.0/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py
--rw-r--r--   0        0        0     3152 2023-04-23 04:17:26.732344 twitter_api_py-0.1.0/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py
--rw-r--r--   0        0        0      669 2023-04-23 01:30:29.708648 twitter_api_py-0.1.0/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py
--rw-r--r--   0        0        0     1236 2023-04-23 01:38:25.292630 twitter_api_py-0.1.0/twitter_api/rate_limit/manager/rate_limit_manager.py
--rw-r--r--   0        0        0     3461 2023-04-23 01:38:25.302629 twitter_api_py-0.1.0/twitter_api/rate_limit/rate_limit.py
--rw-r--r--   0        0        0      291 2023-04-22 15:58:08.574544 twitter_api_py-0.1.0/twitter_api/rate_limit/rate_limit_info.py
--rw-r--r--   0        0        0       91 2023-04-02 10:14:57.836343 twitter_api_py-0.1.0/twitter_api/rate_limit/rate_limit_target.py
--rw-r--r--   0        0        0        0 2023-04-01 17:37:01.267513 twitter_api_py-0.1.0/twitter_api/types/__init__.py
--rw-r--r--   0        0        0      386 2023-04-09 09:46:11.323030 twitter_api_py-0.1.0/twitter_api/types/chainable.py
--rw-r--r--   0        0        0      696 2023-04-09 09:46:11.323030 twitter_api_py-0.1.0/twitter_api/types/comma_separatable.py
--rw-r--r--   0        0        0      234 2023-04-02 10:01:26.462016 twitter_api_py-0.1.0/twitter_api/types/endpoint.py
--rw-r--r--   0        0        0     1580 2023-04-09 12:23:51.244202 twitter_api_py-0.1.0/twitter_api/types/extra_permissive_model.py
--rw-r--r--   0        0        0      632 2023-04-22 12:33:08.907581 twitter_api_py-0.1.0/twitter_api/types/http.py
--rw-r--r--   0        0        0     2362 2023-04-20 12:43:51.415589 twitter_api_py-0.1.0/twitter_api/types/model.py
--rw-r--r--   0        0        0     2325 2023-04-12 13:08:15.038787 twitter_api_py-0.1.0/twitter_api/types/oauth.py
--rw-r--r--   0        0        0     3175 2023-04-22 17:10:32.168434 twitter_api_py-0.1.0/twitter_api/types/paging.py
--rw-r--r--   0        0        0       58 2023-04-01 09:17:10.085603 twitter_api_py-0.1.0/twitter_api/types/screen_name.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:10.085603 twitter_api_py-0.1.0/twitter_api/utils/__init__.py
--rw-r--r--   0        0        0      123 2023-04-09 09:46:44.433033 twitter_api_py-0.1.0/twitter_api/utils/datetime.py
--rw-r--r--   0        0        0      241 2023-04-02 07:14:34.472553 twitter_api_py-0.1.0/twitter_api/utils/functional.py
--rw-r--r--   0        0        0      952 2023-04-17 13:51:30.147495 twitter_api_py-0.1.0/twitter_api/utils/json.py
--rw-r--r--   0        0        0        0 2023-04-22 15:06:46.107533 twitter_api_py-0.1.0/twitter_api/utils/logger.py
--rw-r--r--   0        0        0      890 2023-04-22 10:21:01.811509 twitter_api_py-0.1.0/twitter_api/utils/oauth.py
--rw-r--r--   0        0        0      603 2023-04-23 01:13:48.991718 twitter_api_py-0.1.0/twitter_api/warning.py
--rw-r--r--   0        0        0     2778 1970-01-01 00:00:00.000000 twitter_api_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2159 2023-04-26 11:13:09.330123 twitter_api_py-0.2.0/README.md
+-rw-r--r--   0        0        0     1516 2023-05-01 05:35:27.146293 twitter_api_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      480 2023-05-01 05:34:09.265632 twitter_api_py-0.2.0/twitter_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-01 09:17:09.975602 twitter_api_py-0.2.0/twitter_api/api/__init__.py
+-rw-r--r--   0        0        0      281 2023-04-22 04:51:08.637342 twitter_api_py-0.2.0/twitter_api/api/resources/api_resources.py
+-rw-r--r--   0        0        0      437 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/oauth2_invalidate_token/__init__.py
+-rw-r--r--   0        0        0     2299 2023-04-24 16:07:45.386094 twitter_api_py-0.2.0/twitter_api/api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py
+-rw-r--r--   0        0        0      332 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/oauth2_token/__init__.py
+-rw-r--r--   0        0        0     2191 2023-04-24 16:08:44.345977 twitter_api_py-0.2.0/twitter_api/api/resources/oauth2_token/post_oauth2_token.py
+-rw-r--r--   0        0        0      541 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversation_messages/__init__.py
+-rw-r--r--   0        0        0     2336 2023-04-24 16:07:45.566094 twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py
+-rw-r--r--   0        0        0      441 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations/__init__.py
+-rw-r--r--   0        0        0     2184 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations/post_v2_dm_conversations.py
+-rw-r--r--   0        0        0      673 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py
+-rw-r--r--   0        0        0     8955 2023-04-27 14:28:44.152903 twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py
+-rw-r--r--   0        0        0      676 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations_with_participant_messages/__init__.py
+-rw-r--r--   0        0        0     2410 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py
+-rw-r--r--   0        0        0      429 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweet/__init__.py
+-rw-r--r--   0        0        0     1450 2023-04-24 12:44:19.060255 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweet/delete_v2_tweet.py
+-rw-r--r--   0        0        0     3128 2023-04-27 14:28:44.152903 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweet/get_v2_tweet.py
+-rw-r--r--   0        0        0      458 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweet_retweeted_by/__init__.py
+-rw-r--r--   0        0        0     6593 2023-04-27 14:28:44.152903 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py
+-rw-r--r--   0        0        0      428 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets/__init__.py
+-rw-r--r--   0        0        0     3017 2023-04-27 14:28:44.152903 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets/get_v2_tweets.py
+-rw-r--r--   0        0        0     2954 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets/post_v2_tweets.py
+-rw-r--r--   0        0        0      438 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_all/__init__.py
+-rw-r--r--   0        0        0     5944 2023-04-27 14:28:44.152903 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py
+-rw-r--r--   0        0        0      471 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_recent/__init__.py
+-rw-r--r--   0        0        0     6043 2023-04-27 14:28:44.152903 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py
+-rw-r--r--   0        0        0      471 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream/__init__.py
+-rw-r--r--   0        0        0     3522 2023-04-27 14:28:44.152903 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py
+-rw-r--r--   0        0        0      770 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream_rules/__init__.py
+-rw-r--r--   0        0        0     2123 2023-04-24 16:07:45.546094 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py
+-rw-r--r--   0        0        0     3099 2023-04-24 16:07:45.616093 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py
+-rw-r--r--   0        0        0      275 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user/__init__.py
+-rw-r--r--   0        0        0     2812 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user/get_v2_user.py
+-rw-r--r--   0        0        0      371 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_followers/__init__.py
+-rw-r--r--   0        0        0     6542 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_followers/get_v2_user_followers.py
+-rw-r--r--   0        0        0      376 2023-04-22 10:21:01.811509 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_following/__init__.py
+-rw-r--r--   0        0        0     1921 2023-04-24 16:07:45.656093 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_following/post_v2_user_following.py
+-rw-r--r--   0        0        0      391 2023-04-22 10:21:01.811509 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_liked_tweets/__init__.py
+-rw-r--r--   0        0        0     7987 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py
+-rw-r--r--   0        0        0      367 2023-04-22 10:21:01.811509 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_retweets/__init__.py
+-rw-r--r--   0        0        0     1927 2023-04-24 16:07:45.706093 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_retweets/post_v2_user_retweets.py
+-rw-r--r--   0        0        0      331 2023-04-22 10:21:01.811509 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_tweets/__init__.py
+-rw-r--r--   0        0        0     8404 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_tweets/get_v2_user_tweets.py
+-rw-r--r--   0        0        0      279 2023-04-22 10:21:01.811509 twitter_api_py-0.2.0/twitter_api/api/resources/v2_users/__init__.py
+-rw-r--r--   0        0        0     2712 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_users/get_v2_users.py
+-rw-r--r--   0        0        0      299 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_users_by/__init__.py
+-rw-r--r--   0        0        0     2787 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_users_by/get_v2_users_by.py
+-rw-r--r--   0        0        0      396 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_users_by_username/__init__.py
+-rw-r--r--   0        0        0     3057 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_users_by_username/get_v2_users_by_username.py
+-rw-r--r--   0        0        0        0 2023-04-01 09:17:10.025603 twitter_api_py-0.2.0/twitter_api/api/types/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 17:04:18.882718 twitter_api_py-0.2.0/twitter_api/api/types/oauth1/__init__.py
+-rw-r--r--   0        0        0      843 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/api/types/oauth1/oauth1_access_token.py
+-rw-r--r--   0        0        0     2825 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/api/types/oauth1/oauth1_authorization.py
+-rw-r--r--   0        0        0        0 2023-04-09 09:46:11.323030 twitter_api_py-0.2.0/twitter_api/api/types/oauth2/__init__.py
+-rw-r--r--   0        0        0      856 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/api/types/oauth2/oauth2_access_token.py
+-rw-r--r--   0        0        0     2855 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/api/types/oauth2/oauth2_authorization.py
+-rw-r--r--   0        0        0       63 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/types/pagination_token.py
+-rw-r--r--   0        0        0        0 2023-04-04 00:14:28.746398 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_conversation/__init__.py
+-rw-r--r--   0        0        0      345 2023-04-09 09:46:44.353033 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_conversation/dm_conversation.py
+-rw-r--r--   0        0        0      205 2023-04-04 14:28:03.516388 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_conversation/dm_conversation_attachment.py
+-rw-r--r--   0        0        0       64 2023-04-04 00:15:15.770562 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_conversation/dm_conversation_id.py
+-rw-r--r--   0        0        0      598 2023-04-05 12:42:42.545017 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_conversation/dm_conversation_message.py
+-rw-r--r--   0        0        0        0 2023-04-04 00:15:59.434445 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_event/__init__.py
+-rw-r--r--   0        0        0      331 2023-04-25 14:01:08.860602 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_event/dm_event_expansion.py
+-rw-r--r--   0        0        0      437 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_event/dm_event_field.py
+-rw-r--r--   0        0        0       57 2023-04-04 00:16:14.175754 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_event/dm_event_id.py
+-rw-r--r--   0        0        0      238 2023-04-25 13:49:11.742866 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_event/dm_event_type.py
+-rw-r--r--   0        0        0      315 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/types/v2_domain.py
+-rw-r--r--   0        0        0      248 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/types/v2_entity.py
+-rw-r--r--   0        0        0        0 2023-04-15 05:54:42.060789 twitter_api_py-0.2.0/twitter_api/api/types/v2_geo/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-15 05:55:44.170800 twitter_api_py-0.2.0/twitter_api/api/types/v2_geo/geo.py
+-rw-r--r--   0        0        0        0 2023-04-01 09:17:10.035603 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/__init__.py
+-rw-r--r--   0        0        0     1389 2023-04-15 06:07:09.620870 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media.py
+-rw-r--r--   0        0        0      570 2023-04-15 15:58:56.812733 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_field.py
+-rw-r--r--   0        0        0      100 2023-04-01 16:14:08.728923 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_id.py
+-rw-r--r--   0        0        0       56 2023-04-01 09:17:10.035603 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_key.py
+-rw-r--r--   0        0        0      376 2023-04-15 06:00:40.800828 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_non_public_metrics.py
+-rw-r--r--   0        0        0      411 2023-04-15 06:02:11.910834 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_organic_metrics.py
+-rw-r--r--   0        0        0      412 2023-04-15 06:03:23.150843 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_promoted_metrics.py
+-rw-r--r--   0        0        0      190 2023-04-15 06:04:09.220847 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_public_metrics.py
+-rw-r--r--   0        0        0      211 2023-04-15 06:06:05.030862 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_variants.py
+-rw-r--r--   0        0        0        0 2023-04-01 09:17:10.035603 twitter_api_py-0.2.0/twitter_api/api/types/v2_place/__init__.py
+-rw-r--r--   0        0        0      643 2023-04-15 05:56:35.000801 twitter_api_py-0.2.0/twitter_api/api/types/v2_place/place.py
+-rw-r--r--   0        0        0      348 2023-04-15 15:58:30.892600 twitter_api_py-0.2.0/twitter_api/api/types/v2_place/place_field.py
+-rw-r--r--   0        0        0       94 2023-04-01 09:17:10.045603 twitter_api_py-0.2.0/twitter_api/api/types/v2_place/place_id.py
+-rw-r--r--   0        0        0        0 2023-04-01 09:17:10.045603 twitter_api_py-0.2.0/twitter_api/api/types/v2_poll/__init__.py
+-rw-r--r--   0        0        0      601 2023-04-15 06:10:52.180889 twitter_api_py-0.2.0/twitter_api/api/types/v2_poll/poll.py
+-rw-r--r--   0        0        0      272 2023-04-15 15:58:36.582629 twitter_api_py-0.2.0/twitter_api/api/types/v2_poll/poll_field.py
+-rw-r--r--   0        0        0       54 2023-04-01 09:17:10.045603 twitter_api_py-0.2.0/twitter_api/api/types/v2_poll/poll_id.py
+-rw-r--r--   0        0        0      164 2023-04-15 06:09:28.320883 twitter_api_py-0.2.0/twitter_api/api/types/v2_poll/poll_option.py
+-rw-r--r--   0        0        0        0 2023-04-02 02:04:07.967716 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/__init__.py
+-rw-r--r--   0        0        0     1179 2023-04-04 14:56:44.417296 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet.py
+-rw-r--r--   0        0        0      400 2023-04-04 14:28:04.506389 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_entities.py
+-rw-r--r--   0        0        0      929 2023-04-04 14:28:04.676389 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_entities_description.py
+-rw-r--r--   0        0        0      184 2023-04-24 13:31:22.645664 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_entities_description_cashtag.py
+-rw-r--r--   0        0        0      184 2023-04-23 16:29:08.693648 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_entities_description_hashtag.py
+-rw-r--r--   0        0        0      250 2023-04-04 14:57:14.027308 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_entities_description_mention.py
+-rw-r--r--   0        0        0      258 2023-04-02 02:13:19.847028 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_entities_description_url.py
+-rw-r--r--   0        0        0      338 2023-04-02 02:10:33.754809 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_entities_url.py
+-rw-r--r--   0        0        0      258 2023-04-10 15:48:58.984612 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_includes.py
+-rw-r--r--   0        0        0      219 2023-04-02 02:26:55.269961 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_public_metrics.py
+-rw-r--r--   0        0        0      352 2023-04-02 02:04:56.864520 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_withheld.py
+-rw-r--r--   0        0        0        0 2023-04-09 09:46:44.373033 twitter_api_py-0.2.0/twitter_api/api/types/v2_rule/__init__.py
+-rw-r--r--   0        0        0      319 2023-04-09 09:46:44.433033 twitter_api_py-0.2.0/twitter_api/api/types/v2_rule/rule.py
+-rw-r--r--   0        0        0       54 2023-04-09 09:46:44.373033 twitter_api_py-0.2.0/twitter_api/api/types/v2_rule/rule_id.py
+-rw-r--r--   0        0        0       55 2023-04-09 09:46:44.433033 twitter_api_py-0.2.0/twitter_api/api/types/v2_rule/rule_tag.py
+-rw-r--r--   0        0        0     1411 2023-04-23 06:01:36.209583 twitter_api_py-0.2.0/twitter_api/api/types/v2_scope.py
+-rw-r--r--   0        0        0        0 2023-04-01 09:17:10.045603 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/__init__.py
+-rw-r--r--   0        0        0     6442 2023-04-18 13:43:34.885017 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet.py
+-rw-r--r--   0        0        0      309 2023-04-04 14:19:50.365994 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_attachments.py
+-rw-r--r--   0        0        0      229 2023-04-04 14:30:09.146468 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_context_annotation.py
+-rw-r--r--   0        0        0      314 2023-04-01 09:17:36.515599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_edit_controls.py
+-rw-r--r--   0        0        0      720 2023-04-01 09:17:36.415599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_entities.py
+-rw-r--r--   0        0        0      333 2023-04-01 09:17:36.415599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_entities_annotation.py
+-rw-r--r--   0        0        0      247 2023-04-01 09:17:36.415599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_entities_cashtag.py
+-rw-r--r--   0        0        0      247 2023-04-01 09:17:36.415599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_entities_hashtag.py
+-rw-r--r--   0        0        0      317 2023-04-04 14:57:19.327310 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_entities_mention.py
+-rw-r--r--   0        0        0      415 2023-04-15 03:52:45.757502 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_entities_url.py
+-rw-r--r--   0        0        0      632 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_expansion.py
+-rw-r--r--   0        0        0     1910 2023-04-23 06:33:19.778673 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_field.py
+-rw-r--r--   0        0        0      288 2023-04-01 09:17:36.415599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_geo.py
+-rw-r--r--   0        0        0      231 2023-04-01 09:17:37.035599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_geo_coordinates.py
+-rw-r--r--   0        0        0      100 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_id.py
+-rw-r--r--   0        0        0      287 2023-04-01 09:17:37.035599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_non_public_metrics.py
+-rw-r--r--   0        0        0      285 2023-04-01 09:17:36.415599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_organic_metrics.py
+-rw-r--r--   0        0        0      286 2023-04-01 09:17:36.415599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_promoted_metrics.py
+-rw-r--r--   0        0        0      437 2023-04-09 15:28:28.034225 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_public_metrics.py
+-rw-r--r--   0        0        0      256 2023-04-15 10:39:45.485596 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_referenced_tweet.py
+-rw-r--r--   0        0        0     6983 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_response_body.py
+-rw-r--r--   0        0        0      387 2023-04-02 01:59:57.044158 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_withheld.py
+-rw-r--r--   0        0        0        0 2023-04-01 09:17:10.065603 twitter_api_py-0.2.0/twitter_api/api/types/v2_user/__init__.py
+-rw-r--r--   0        0        0      977 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/types/v2_user/user.py
+-rw-r--r--   0        0        0      157 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/types/v2_user/user_expantion.py
+-rw-r--r--   0        0        0      608 2023-04-15 16:00:19.963155 twitter_api_py-0.2.0/twitter_api/api/types/v2_user/user_field.py
+-rw-r--r--   0        0        0       54 2023-04-01 09:17:10.065603 twitter_api_py-0.2.0/twitter_api/api/types/v2_user/user_id.py
+-rw-r--r--   0        0        0       97 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/types/v2_user/user_verified_type.py
+-rw-r--r--   0        0        0      128 2023-04-02 07:41:55.232378 twitter_api_py-0.2.0/twitter_api/api/types/v2_user/username.py
+-rw-r--r--   0        0        0        0 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/__init__.py
+-rw-r--r--   0        0        0     1039 2023-05-01 05:03:58.580612 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py
+-rw-r--r--   0        0        0      310 2023-05-01 05:01:04.629161 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth1_access_token_mock_client.py
+-rw-r--r--   0        0        0     1380 2023-05-01 05:01:51.409552 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py
+-rw-r--r--   0        0        0      305 2023-05-01 05:01:45.139500 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth1_authorization_mock_client.py
+-rw-r--r--   0        0        0      806 2023-05-01 05:02:17.969774 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py
+-rw-r--r--   0        0        0      314 2023-05-01 05:02:27.359852 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_mock_client.py
+-rw-r--r--   0        0        0     1209 2023-05-01 05:02:59.990124 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py
+-rw-r--r--   0        0        0      310 2023-05-01 05:03:15.690255 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth2_access_token_mock_client.py
+-rw-r--r--   0        0        0      829 2023-05-01 05:03:36.810430 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py
+-rw-r--r--   0        0        0      305 2023-05-01 05:03:51.400552 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_mock_client.py
+-rw-r--r--   0        0        0        0 2023-04-09 09:46:11.283030 twitter_api_py-0.2.0/twitter_api/client/oauth_session/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/__init__.py
+-rw-r--r--   0        0        0      364 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_access_token/__init__.py
+-rw-r--r--   0        0        0     1143 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py
+-rw-r--r--   0        0        0      450 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/__init__.py
+-rw-r--r--   0        0        0      801 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py
+-rw-r--r--   0        0        0      432 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_authorize/__init__.py
+-rw-r--r--   0        0        0      721 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py
+-rw-r--r--   0        0        0      391 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_request_token/__init__.py
+-rw-r--r--   0        0        0      797 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py
+-rw-r--r--   0        0        0      500 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth2_authorize/__init__.py
+-rw-r--r--   0        0        0      759 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py
+-rw-r--r--   0        0        0      647 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/session_resources.py
+-rw-r--r--   0        0        0      375 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/__init__.py
+-rw-r--r--   0        0        0     1599 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py
+-rw-r--r--   0        0        0     1940 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py
+-rw-r--r--   0        0        0     4048 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth1_real_session.py
+-rw-r--r--   0        0        0     1546 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth1_session.py
+-rw-r--r--   0        0        0     1681 2023-05-01 04:37:46.697568 twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py
+-rw-r--r--   0        0        0     3519 2023-04-30 18:13:50.196233 twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth2_real_session.py
+-rw-r--r--   0        0        0     1030 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth2_session.py
+-rw-r--r--   0        0        0        0 2023-04-01 17:37:10.337565 twitter_api_py-0.2.0/twitter_api/client/request/__init__.py
+-rw-r--r--   0        0        0     1577 2023-04-24 12:44:19.060255 twitter_api_py-0.2.0/twitter_api/client/request/request_async_client.py
+-rw-r--r--   0        0        0      236 2023-04-22 10:21:01.811509 twitter_api_py-0.2.0/twitter_api/client/request/request_async_mock_client.py
+-rw-r--r--   0        0        0     5357 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/request/request_async_real_client.py
+-rw-r--r--   0        0        0     1973 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/client/request/request_client.py
+-rw-r--r--   0        0        0     3316 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/client/request/request_mock_client.py
+-rw-r--r--   0        0        0     7427 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/request/request_real_client.py
+-rw-r--r--   0        0        0    32408 2023-05-01 04:10:39.294049 twitter_api_py-0.2.0/twitter_api/client/twitter_api_async_client.py
+-rw-r--r--   0        0        0    14522 2023-05-01 05:15:05.866148 twitter_api_py-0.2.0/twitter_api/client/twitter_api_async_mock_client.py
+-rw-r--r--   0        0        0    14747 2023-05-01 04:55:52.126573 twitter_api_py-0.2.0/twitter_api/client/twitter_api_async_real_client.py
+-rw-r--r--   0        0        0    32167 2023-05-01 05:09:26.123325 twitter_api_py-0.2.0/twitter_api/client/twitter_api_client.py
+-rw-r--r--   0        0        0    27102 2023-05-01 05:11:36.014406 twitter_api_py-0.2.0/twitter_api/client/twitter_api_mock_client.py
+-rw-r--r--   0        0        0    13587 2023-05-01 04:54:04.605683 twitter_api_py-0.2.0/twitter_api/client/twitter_api_real_client.py
+-rw-r--r--   0        0        0    10799 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/error.py
+-rw-r--r--   0        0        0        0 2023-04-02 08:29:19.122099 twitter_api_py-0.2.0/twitter_api/rate_limit/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/manager/__init__.py
+-rw-r--r--   0        0        0     2238 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/rate_limit/manager/dict_rate_limit_manager.py
+-rw-r--r--   0        0        0      525 2023-04-23 01:32:37.383610 twitter_api_py-0.2.0/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py
+-rw-r--r--   0        0        0        0 2023-04-23 01:25:28.771650 twitter_api_py-0.2.0/twitter_api/rate_limit/manager/handlers/__init__.py
+-rw-r--r--   0        0        0     1296 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py
+-rw-r--r--   0        0        0     3040 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py
+-rw-r--r--   0        0        0      675 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py
+-rw-r--r--   0        0        0     1242 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/manager/rate_limit_manager.py
+-rw-r--r--   0        0        0     3424 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/rate_limit.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/types/__init__.py
+-rw-r--r--   0        0        0      297 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/types/rate_limit_info.py
+-rw-r--r--   0        0        0       91 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/types/rate_limit_target.py
+-rw-r--r--   0        0        0        0 2023-04-01 17:37:01.267513 twitter_api_py-0.2.0/twitter_api/types/__init__.py
+-rw-r--r--   0        0        0      386 2023-04-09 09:46:11.323030 twitter_api_py-0.2.0/twitter_api/types/chainable.py
+-rw-r--r--   0        0        0      697 2023-04-26 11:13:40.460129 twitter_api_py-0.2.0/twitter_api/types/comma_separatable.py
+-rw-r--r--   0        0        0      234 2023-04-02 10:01:26.462016 twitter_api_py-0.2.0/twitter_api/types/endpoint.py
+-rw-r--r--   0        0        0     1580 2023-04-24 17:04:45.312148 twitter_api_py-0.2.0/twitter_api/types/extra_permissive_model.py
+-rw-r--r--   0        0        0      570 2023-04-30 18:19:53.998491 twitter_api_py-0.2.0/twitter_api/types/generic_client.py
+-rw-r--r--   0        0        0      616 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/types/http.py
+-rw-r--r--   0        0        0      734 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/types/httpx.py
+-rw-r--r--   0        0        0     2362 2023-04-20 12:43:51.415589 twitter_api_py-0.2.0/twitter_api/types/model.py
+-rw-r--r--   0        0        0     1742 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/types/oauth.py
+-rw-r--r--   0        0        0     3531 2023-04-30 17:48:26.846710 twitter_api_py-0.2.0/twitter_api/types/paging.py
+-rw-r--r--   0        0        0        0 2023-04-01 09:17:10.085603 twitter_api_py-0.2.0/twitter_api/utils/__init__.py
+-rw-r--r--   0        0        0      123 2023-04-23 15:17:02.699271 twitter_api_py-0.2.0/twitter_api/utils/_datetime.py
+-rw-r--r--   0        0        0      716 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/utils/_functional.py
+-rw-r--r--   0        0        0      904 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/utils/_oauth.py
+-rw-r--r--   0        0        0      775 2023-05-01 04:02:26.399958 twitter_api_py-0.2.0/twitter_api/utils/json.py
+-rw-r--r--   0        0        0      637 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/warning.py
+-rw-r--r--   0        0        0     3106 1970-01-01 00:00:00.000000 twitter_api_py-0.2.0/PKG-INFO
```

### Comparing `twitter_api_py-0.1.0/README.md` & `twitter_api_py-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # <p align="center">✨✨ Twitter API Client by Typed Python ✨✨</p>
 
 <p align="center">
     <a href="https://github.com/yassun4dev/twitter-api-py/actions">
         <img src="https://github.com/yassun4dev/twitter-api-py/actions/workflows/test-suite.yml/badge.svg" alt="Test Suite">
     </a>
+    <a href="https://pypi.org/project/twitter_api_py/">
+        <img src="https://badge.fury.io/py/twitter_api_py.svg" alt="Package version">
+    </a>
 </p>
 
 ![demo](https://raw.githubusercontent.com/yassun4dev/twitter-api-py/main/images/demo.gif)
 
 ## Install
 
 ```sh
@@ -21,30 +24,29 @@
 - Sync / Async Client support.
 - Mock Client support.
 
 
 ## Usage
 The simplest way to use the library is as follows:
 
-As a characteristic feature of the library, it explicitly prompts the user to write the Endpoint URL, which makes it clear from the source code which Twitter API is being called.
-
 ```python
 from twitter_api import TwitterApiClient
 
-twitter_client = TwitterApiClient.from_oauth2_app_env()
-
-response = (
-    twitter_client.resource("https://api.twitter.com/2/tweets")
-    .get({
-        "ids": "1460323737035677698",
-        "expansions": ["referenced_tweets.id"]
-    })
-)
+with TwitterApiClient.from_oauth2_app_env() as twitter_client:
+    response_body = (
+        twitter_client.request("https://api.twitter.com/2/tweets")
+        .get({
+            "ids": "1460323737035677698",
+            "expansions": ["referenced_tweets.id"]
+        })
+    )
 ```
 
+As a characteristic feature of the library, it explicitly prompts the user to write the Endpoint URL, which makes it clear from the source code which Twitter API is being called.
+
 ## Test Code
 
 A mock client is provided by the library to simplify the writing of test code.
 
 This client has the same interface as TwitterApiClient/TwitterApiAsyncClient, and also provides methods (`inject_*_response_body`) for injecting test data.
 
 ```python
@@ -53,16 +55,14 @@
 
 def your_logic(twitter_client: TwitterApiClient):
     ...
 
 def test_your_logic():
     twitter_client = (
         TwitterApiMockClient.from_oauth2_app_env()
-        .inject_post_response_body("https://api.twitter.com/2/tweets", post_response)
-        .inject_get_response_body("https://api.twitter.com/2/tweets/:id", get_response)
-        .inject_delete_response_body("https://api.twitter.com/2/tweets", delete_response)
+        .inject_post_response_body("https://api.twitter.com/2/tweets", post_response_body)
+        .inject_get_response_body("https://api.twitter.com/2/tweets/:id", get_response_body)
+        .inject_delete_response_body("https://api.twitter.com/2/tweets", delete_response_body)
     )
 
     assert your_logic(twitter_client) is True
 ```
-
-
```

### Comparing `twitter_api_py-0.1.0/pyproject.toml` & `twitter_api_py-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 authors = ["yassun4dev <yassun4dev@outlook.com>"]
 description = "Twitter API Client by Typed Python."
 name = "twitter-api-py"
 packages = [{include = "twitter_api"}]
 readme = "README.md"
-version = "0.1.0"
+version = "0.2.0"
 license = "BSD-3-Clause"
+repository = "https://github.com/yassun4dev/twitter-api-py"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
@@ -51,14 +52,15 @@
 
 [tool.flake8]
 max-line-length = 200
 
 [tool.pyright]
 exclude = ["**/__pycache__"]
 reportPrivateImportUsage = "none"
+reportUnusedImport = true
 
 [tool.mypy]
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = [
   "colorama",
   "authlib",
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import base64
-from typing import Literal, TypedDict
+from typing import TypedDict
 
 from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.client.request.request_client import RequestClient
 from twitter_api.error import TwitterApiOAuthVersionWrong
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.http import downcast_dict
 from twitter_api.types.oauth import AccessToken, ApiKey, ApiSecret
 
 ENDPOINT: Endpoint = Endpoint("POST", "https://api.twitter.com/oauth2/invalidate_token")
@@ -43,15 +42,15 @@
 
         bearer_token = base64.b64encode(
             f"{api_key}:{api_secret}".encode(),
         )
 
         return self.request_client.post(
             endpoint=ENDPOINT,
-            response_type=PostOauth2InvalidateTokenResponseBody,
+            response_body_type=PostOauth2InvalidateTokenResponseBody,
             auth=False,
             headers={
                 "Authorization": f"Basic {bearer_token.decode()}",
                 "Content-Type": "application/x-www-form-urlencoded",
             },
             query=downcast_dict(query),
         )
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/oauth2_token/post_oauth2_token.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/oauth2_token/post_oauth2_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
         bearer_token = base64.b64encode(
             f"{api_key}:{api_secret}".encode(),
         )
 
         return self.request_client.post(
             endpoint=ENDPOINT,
-            response_type=PostOauth2TokenResponseBody,
+            response_body_type=PostOauth2TokenResponseBody,
             auth=False,
             headers={
                 "Authorization": f"Basic {bearer_token.decode()}",
                 "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
             },
             query=downcast_dict(query),
         )
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_dm_conversation_messages/__init__.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversation_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         refer: https://developer.twitter.com/en/docs/twitter-api/direct-messages/manage/api-reference/post-dm_conversations-dm_conversation_id-messages
         """
         return self.request_client.post(
             endpoint=ENDPOINT,
             url=ENDPOINT.url.replace(":dm_conversation_id", dm_conversation_id),
             body=downcast_dict(request_body),
-            response_type=PostV2DmConversationMessagesResponseBody,
+            response_body_type=PostV2DmConversationMessagesResponseBody,
         )
 
 
 class AsyncPostV2DmConversationMessagesResources(PostV2DmConversationMessagesResources):
     async def post(
         self,
         dm_conversation_id: DmConversationId,
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_dm_conversations/post_v2_dm_conversations.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations/post_v2_dm_conversations.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,32 +37,29 @@
         "users.read",
     )
     @rate_limit(ENDPOINT, "user", requests=200, mins=15)
     @rate_limit(ENDPOINT, "user", requests=1000, hours=24)
     @rate_limit(ENDPOINT, "app", requests=15000, hours=24)
     def post(
         self,
-        participant_id: UserId,
         request_body: PostV2DmConversationsRequestBody,
     ) -> PostV2DmConversationsResponseBody:
         """
         DM 用の新しい会話グループを作成する。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/direct-messages/manage/api-reference/post-dm_conversations
         """
         return self.request_client.post(
             endpoint=ENDPOINT,
             body=downcast_dict(request_body),
-            response_type=PostV2DmConversationsResponseBody,
+            response_body_type=PostV2DmConversationsResponseBody,
         )
 
 
 class AsyncPostV2DmConversationsResources(PostV2DmConversationsResources):
     async def post(
         self,
-        participant_id: UserId,
         request_body: PostV2DmConversationsRequestBody,
     ) -> PostV2DmConversationsResponseBody:
         return super().post(
-            participant_id,
             request_body,
         )
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_dm_conversations_with_messages/__init__.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations_with_participant_messages/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TypeAlias
 
 from typing_extensions import Literal
 
-from .post_v2_dm_conversations_with_messages import (
+from .post_v2_dm_conversations_with_participant_messages import (
     AsyncPostV2DmConversationsWithParticipantMessagesResources,
     PostV2DmConversationsWithParticipantMessagesResources,
 )
 
 V2DmConversationsWithParticipantMessagesUrl: TypeAlias = Literal[
     "https://api.twitter.com/2/dm_conversations/with/:participant_id/messages"
 ]
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_dm_conversations_with_messages/post_v2_dm_conversations_with_messages.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         refer: https://developer.twitter.com/en/docs/twitter-api/direct-messages/manage/api-reference/post-dm_conversations-with-participant_id-messages
         """
         return self.request_client.post(
             endpoint=ENDPOINT,
             url=ENDPOINT.url.replace(":participant_id", participant_id),
             body=downcast_dict(request_body),
-            response_type=PostV2DmConversationsWithParticipantMessagesResponseBody,
+            response_body_type=PostV2DmConversationsWithParticipantMessagesResponseBody,
         )
 
 
 class AsyncPostV2DmConversationsWithParticipantMessagesResources(
     PostV2DmConversationsWithParticipantMessagesResources
 ):
     async def post(
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweet/delete_v2_tweet.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweet/delete_v2_tweet.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         """
         ツイートを削除する。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/manage-tweets/api-reference/delete-tweets-id
         """
         return self.request_client.delete(
             endpoint=ENDPOINT,
-            response_type=DeleteV2TweetResponseBody,
+            response_body_type=DeleteV2TweetResponseBody,
             url=ENDPOINT.url.replace(":id", id),
         )
 
 
 class AsyncDeleteV2TweetResources(DeleteV2TweetResources):
     async def delete(
         self,
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweet/get_v2_tweet.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweet/get_v2_tweet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import NotRequired, Optional, TypedDict
 
 from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_expansion import Expansion
 from twitter_api.api.types.v2_media.media_field import MediaField
 from twitter_api.api.types.v2_place.place_field import PlaceField
 from twitter_api.api.types.v2_poll.poll_field import PollField
 from twitter_api.api.types.v2_scope import oauth2_scopes
+from twitter_api.api.types.v2_tweet.tweet_expansion import TweetExpansion
 from twitter_api.api.types.v2_tweet.tweet_field import TweetField
 from twitter_api.api.types.v2_tweet.tweet_id import TweetId
 from twitter_api.api.types.v2_tweet.tweet_response_body import TweetResponseBody
 from twitter_api.api.types.v2_user.user_field import UserField
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets/:id")
 
 GetV2TweetQueryParameters = TypedDict(
     "GetV2TweetQueryParameters",
     {
-        "expansions": NotRequired[Optional[CommaSeparatable[Expansion]]],
+        "expansions": NotRequired[Optional[CommaSeparatable[TweetExpansion]]],
         "media.fields": NotRequired[Optional[CommaSeparatable[MediaField]]],
         "place.fields": NotRequired[Optional[CommaSeparatable[PlaceField]]],
         "poll.fields": NotRequired[Optional[CommaSeparatable[PollField]]],
         "tweet.fields": NotRequired[Optional[CommaSeparatable[TweetField]]],
         "user.fields": NotRequired[Optional[CommaSeparatable[UserField]]],
     },
 )
@@ -64,15 +64,15 @@
         """
         ツイートを取得する。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/lookup/api-reference/get-tweets-id
         """
         return self.request_client.get(
             endpoint=ENDPOINT,
-            response_type=GetV2TweetResponseBody,
+            response_body_type=GetV2TweetResponseBody,
             url=ENDPOINT.url.replace(":id", id),
             query=_make_query(query),
         )
 
 
 class AsyncGetV2TweetResources(GetV2TweetResources):
     async def get(
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from functools import partial
 from typing import AsyncGenerator, Generator, NotRequired, Optional, Self, TypedDict
 
 from pydantic import Field
 
 from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_expansion import Expansion
+from twitter_api.api.types.pagination_token import PaginationToken
 from twitter_api.api.types.v2_retweet.retweet import Retweet
 from twitter_api.api.types.v2_scope import oauth2_scopes
 from twitter_api.api.types.v2_tweet.tweet import Tweet
+from twitter_api.api.types.v2_tweet.tweet_expansion import TweetExpansion
 from twitter_api.api.types.v2_tweet.tweet_field import TweetField
 from twitter_api.api.types.v2_tweet.tweet_id import TweetId
 from twitter_api.api.types.v2_user.user_field import UserField
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.paging import (
     PageResponseBody,
-    get_collected_paging_response_async,
-    get_collected_paging_response_sync,
-    get_paging_response_iter_async,
-    get_paging_response_iter_sync,
+    get_collected_paging_response_body_async,
+    get_collected_paging_response_body_sync,
+    get_paging_response_body_iter_async,
+    get_paging_response_body_iter_sync,
 )
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets/:id/retweeted_by")
 
 GetV2TweetRetweetedByQueryParameters = TypedDict(
     "GetV2TweetRetweetedByQueryParameters",
     {
-        "expansions": NotRequired[Optional[CommaSeparatable[Expansion]]],
+        "expansions": NotRequired[Optional[CommaSeparatable[TweetExpansion]]],
         "max_results": NotRequired[Optional[int]],
         "pagination_token": NotRequired[Optional[str]],
         "tweet.fields": NotRequired[Optional[CommaSeparatable[TweetField]]],
         "user.fields": NotRequired[Optional[CommaSeparatable[UserField]]],
     },
 )
 
@@ -52,16 +53,16 @@
 
     def extend(self, other: Self) -> None:
         self.tweets.extend(other.tweets)
 
 
 class GetV2TweetRetweetedByResponseBodyMeta(ExtraPermissiveModel):
     result_count: int
-    next_token: Optional[str] = None
-    previous_token: Optional[str] = None
+    next_token: Optional[PaginationToken] = None
+    previous_token: Optional[PaginationToken] = None
 
     def extend(self, other: Self) -> None:
         self.result_count += other.result_count
         self.next_token = None
         self.previous_token = None
 
 
@@ -70,15 +71,15 @@
     meta: GetV2TweetRetweetedByResponseBodyMeta
     includes: GetV2TweetRetweetedByResponseBodyIncludes = Field(
         default_factory=GetV2TweetRetweetedByResponseBodyIncludes,
     )
     errors: Optional[list[dict]] = None
 
     @property
-    def meta_next_token(self) -> str | None:
+    def meta_next_token(self) -> PaginationToken | None:
         return self.meta.next_token
 
     def extend(self, other: Self) -> None:
         self.data.extend(other.data)
         self.meta.extend(other.meta)
         self.includes.extend(other.includes)
 
@@ -102,55 +103,63 @@
         """
         リツイートされたツイートの一覧を取得する。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/retweets/api-reference/get-tweets-id-retweeted_by
         """
         return self.request_client.get(
             endpoint=ENDPOINT,
-            response_type=GetV2TweetRetweetedByResponseBody,
+            response_body_type=GetV2TweetRetweetedByResponseBody,
             url=ENDPOINT.url.replace(":id", id),
             query=_make_query(query) if query is not None else None,
         )
 
-    def get_paging_response_iter(
+    def get_paging_response_body_iter(
         self, id: TweetId, query: Optional[GetV2TweetRetweetedByQueryParameters] = None
     ) -> Generator[GetV2TweetRetweetedByResponseBody, None, None]:
         """
         リツイートされたツイートの一覧を取得する。
 
         ページングされた API のレスポンスをイテレータで返す。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/retweets/api-reference/get-tweets-id-retweeted_by
         """
-        return get_paging_response_iter_sync(partial(self.get, id), query)
+        return get_paging_response_body_iter_sync(
+            partial(self.get, id), query, "pagination_token"
+        )
 
-    def get_collected_response(
+    def get_collected_paging_response_body(
         self, id: TweetId, query: Optional[GetV2TweetRetweetedByQueryParameters] = None
     ) -> GetV2TweetRetweetedByResponseBody:
         """
         リツイートされたツイートの一覧を取得する。
 
         ページングされた API のレスポンスをまとめて一つのレスポンスとして返す。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/retweets/api-reference/get-tweets-id-retweeted_by
         """
-        return get_collected_paging_response_sync(partial(self.get, id), query)
+        return get_collected_paging_response_body_sync(
+            partial(self.get, id), query, "pagination_token"
+        )
 
 
 class AsyncGetV2TweetRetweetedByResources(GetV2TweetRetweetedByResources):
     async def get(
         self, id: TweetId, query: Optional[GetV2TweetRetweetedByQueryParameters] = None
     ) -> GetV2TweetRetweetedByResponseBody:
         return super().get(
             id,
             query,
         )
 
-    async def get_paging_response_iter(
+    async def get_paging_response_body_iter(
         self, id: TweetId, query: Optional[GetV2TweetRetweetedByQueryParameters] = None
     ) -> AsyncGenerator[GetV2TweetRetweetedByResponseBody, None]:
-        return get_paging_response_iter_async(partial(self.get, id), query)
+        return get_paging_response_body_iter_async(
+            partial(self.get, id), query, "pagination_token"
+        )
 
-    async def get_collected_response(
+    async def get_collected_paging_response_body(
         self, id: TweetId, query: Optional[GetV2TweetRetweetedByQueryParameters] = None
     ) -> GetV2TweetRetweetedByResponseBody:
-        return await get_collected_paging_response_async(partial(self.get, id), query)
+        return await get_collected_paging_response_body_async(
+            partial(self.get, id), query, "pagination_token"
+        )
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets/get_v2_tweets.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets/get_v2_tweets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from typing import NotRequired, Optional, TypedDict
 
 from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_expansion import Expansion
 from twitter_api.api.types.v2_media.media_field import MediaField
 from twitter_api.api.types.v2_place.place_field import PlaceField
 from twitter_api.api.types.v2_poll.poll_field import PollField
 from twitter_api.api.types.v2_scope import oauth2_scopes
+from twitter_api.api.types.v2_tweet.tweet_expansion import TweetExpansion
 from twitter_api.api.types.v2_tweet.tweet_field import TweetField
 from twitter_api.api.types.v2_tweet.tweet_id import TweetId
 from twitter_api.api.types.v2_tweet.tweet_response_body import TweetsResponseBody
 from twitter_api.api.types.v2_user.user_field import UserField
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets")
 
 GetV2TweetsQueryParameters = TypedDict(
     "GetV2TweetsQueryParameters",
     {
         "ids": CommaSeparatable[TweetId],
-        "expansions": NotRequired[Optional[CommaSeparatable[Expansion]]],
+        "expansions": NotRequired[Optional[CommaSeparatable[TweetExpansion]]],
         "media.fields": NotRequired[Optional[CommaSeparatable[MediaField]]],
         "place.fields": NotRequired[Optional[CommaSeparatable[PlaceField]]],
         "poll.fields": NotRequired[Optional[CommaSeparatable[PollField]]],
         "tweet.fields": NotRequired[Optional[CommaSeparatable[TweetField]]],
         "user.fields": NotRequired[Optional[CommaSeparatable[UserField]]],
     },
 )
@@ -58,14 +58,14 @@
         ツイートの一覧を取得する。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/lookup/api-reference/get-tweets
         """
         return self.request_client.get(
             endpoint=ENDPOINT,
             query=_make_query(query),
-            response_type=GetV2TweetsResponseBody,
+            response_body_type=GetV2TweetsResponseBody,
         )
 
 
 class AsyncGetV2TweetsResources(GetV2TweetsResources):
     async def get(self, query: GetV2TweetsQueryParameters) -> GetV2TweetsResponseBody:
         return super().get(query)
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets/post_v2_tweets.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets/post_v2_tweets.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,30 +31,30 @@
 
 
 class PostV2TweetsReply(TypedDict):
     exclude_reply_user_ids: list[UserId]
     in_reply_to_tweet_id: list[TweetId]
 
 
-class _PostV2TweetsRequestBodyBase(TypedDict):
+class _BasePostV2TweetsRequestBody(TypedDict):
     direct_message_deep_link: NotRequired[Optional[Url]]
     for_super_followers_only: NotRequired[Optional[bool]]
     geo: NotRequired[Optional[PostV2TweetsGeospatialInformation]]
     poll: NotRequired[Optional[PostV2TweetsPoll]]
     quote_tweet_id: NotRequired[Optional[TweetId]]
     reply: NotRequired[Optional[PostV2TweetsReply]]
     reply_settings: NotRequired[Optional[Literal["mentionedUsers", "following"]]]
 
 
-class PostV2TweetsRequestBodyMedia(_PostV2TweetsRequestBodyBase):
+class PostV2TweetsRequestBodyMedia(_BasePostV2TweetsRequestBody):
     text: NotRequired[Optional[str]]
     media: PostV2TweetsMedia
 
 
-class PostV2TweetsRequestBodyText(_PostV2TweetsRequestBodyBase):
+class PostV2TweetsRequestBodyText(_BasePostV2TweetsRequestBody):
     text: str
     media: NotRequired[Optional[PostV2TweetsMedia]]
 
 
 PostV2TweetsRequestBody = Union[
     PostV2TweetsRequestBodyText,
     PostV2TweetsRequestBodyMedia,
@@ -76,15 +76,15 @@
         """
         ツイートする。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/manage-tweets/api-reference/post-tweets
         """
         return self.request_client.post(
             endpoint=ENDPOINT,
-            response_type=PostV2TweetsResponseBody,
+            response_body_type=PostV2TweetsResponseBody,
             body=downcast_dict(request_body),
         )
 
 
 class AsyncPostV2TweetsResources(PostV2TweetsResources):
     async def post(
         self, request_body: PostV2TweetsRequestBody
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,134 +1,135 @@
 from datetime import datetime
 from typing import AsyncGenerator, Generator, Literal, NotRequired, Optional, TypedDict
-from urllib import parse
 
 from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_expansion import Expansion
+from twitter_api.api.types.pagination_token import PaginationToken
 from twitter_api.api.types.v2_media.media_field import MediaField
 from twitter_api.api.types.v2_place.place_field import PlaceField
 from twitter_api.api.types.v2_poll.poll_field import PollField
 from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_search_query import SearchQuery
+from twitter_api.api.types.v2_tweet.tweet_expansion import TweetExpansion
 from twitter_api.api.types.v2_tweet.tweet_field import TweetField
 from twitter_api.api.types.v2_tweet.tweet_id import TweetId
 from twitter_api.api.types.v2_tweet.tweet_response_body import TweetsSearchResponseBody
 from twitter_api.api.types.v2_user.user_field import UserField
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.paging import (
-    get_collected_paging_response_async,
-    get_collected_paging_response_sync,
-    get_paging_response_iter_async,
-    get_paging_response_iter_sync,
+    get_collected_paging_response_body_async,
+    get_collected_paging_response_body_sync,
+    get_paging_response_body_iter_async,
+    get_paging_response_body_iter_sync,
 )
-from twitter_api.utils.datetime import rfc3339
-from twitter_api.utils.functional import map_optional
+from twitter_api.utils._datetime import rfc3339
+from twitter_api.utils._functional import map_optional
 
-ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets/search/all")
+ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets/search/recent")
 
-GetV2TweetsSearchAllQueryParameters = TypedDict(
-    "GetV2TweetsSearchAllQueryParameters",
+GetV2TweetsSearchRecentQueryParameters = TypedDict(
+    "GetV2TweetsSearchRecentQueryParameters",
     {
-        "query": str | SearchQuery,
+        "query": str,
         "start_time": NotRequired[Optional[datetime]],
         "end_time": NotRequired[Optional[datetime]],
         "since_id": NotRequired[Optional[TweetId]],
         "until_id": NotRequired[Optional[TweetId]],
         "sort_order": NotRequired[Optional[Literal["recency", "relevancy"]]],
-        "next_token": NotRequired[Optional[str]],
+        "next_token": NotRequired[Optional[PaginationToken]],
         "max_results": NotRequired[Optional[int]],
-        "expansions": NotRequired[Optional[CommaSeparatable[Expansion]]],
+        "expansions": NotRequired[Optional[CommaSeparatable[TweetExpansion]]],
         "place.fields": NotRequired[Optional[CommaSeparatable[PlaceField]]],
         "media.fields": NotRequired[Optional[CommaSeparatable[MediaField]]],
         "poll.fields": NotRequired[Optional[CommaSeparatable[PollField]]],
         "tweet.fields": NotRequired[Optional[CommaSeparatable[TweetField]]],
         "user.fields": NotRequired[Optional[CommaSeparatable[UserField]]],
     },
 )
 
 
-def _make_query(query: GetV2TweetsSearchAllQueryParameters) -> dict:
+def _make_query(query: GetV2TweetsSearchRecentQueryParameters) -> dict:
     return {
-        "query": parse.quote(str(query["query"])),
+        "query": str(query["query"]),
         "start_time": map_optional(rfc3339, query.get("start_time")),
         "end_time": map_optional(rfc3339, query.get("end_time")),
         "since_id": query.get("since_id"),
         "until_id": query.get("until_id"),
         "sort_order": query.get("sort_order"),
         "next_token": query.get("next_token"),
-        "max_results": query.get("expansions"),
+        "max_results": query.get("max_results"),
         "expansions": comma_separated_str(query.get("expansions")),
-        "place.fields": query.get("place.fields"),
-        "media.fields": query.get("media.fields"),
-        "poll.fields": query.get("poll.fields"),
+        "place.fields": comma_separated_str(query.get("place.fields")),
+        "media.fields": comma_separated_str(query.get("media.fields")),
+        "poll.fields": comma_separated_str(query.get("poll.fields")),
         "tweet.fields": comma_separated_str(query.get("tweet.fields")),
         "user.fields": comma_separated_str(query.get("user.fields")),
     }
 
 
-class GetV2TweetsSearchAllResponseBody(TweetsSearchResponseBody):
+class GetV2TweetsSearchRecentResponseBody(TweetsSearchResponseBody):
     pass
 
 
-class GetV2TweetsSearchAllResources(ApiResources):
+class GetV2TweetsSearchRecentResources(ApiResources):
     @oauth2_scopes(
         "tweet.read",
         "users.read",
     )
-    @rate_limit(ENDPOINT, "app", requests=300, mins=15)
-    @rate_limit(ENDPOINT, "app", requests=1, seconds=1)
+    @rate_limit(ENDPOINT, "app", requests=450, mins=15)
+    @rate_limit(ENDPOINT, "user", requests=180, mins=15)
     def get(
-        self, query: GetV2TweetsSearchAllQueryParameters
-    ) -> GetV2TweetsSearchAllResponseBody:
+        self, query: GetV2TweetsSearchRecentQueryParameters
+    ) -> GetV2TweetsSearchRecentResponseBody:
         """
         ツイートの一覧を検索する。
 
-        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-all
+        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-recent
         """
         return self.request_client.get(
             endpoint=ENDPOINT,
-            response_type=GetV2TweetsSearchAllResponseBody,
+            response_body_type=GetV2TweetsSearchRecentResponseBody,
             query=_make_query(query) if query is not None else None,
         )
 
-    def get_paging_response_iter(
-        self, query: GetV2TweetsSearchAllQueryParameters
-    ) -> Generator[GetV2TweetsSearchAllResponseBody, None, None]:
+    def get_paging_response_body_iter(
+        self, query: GetV2TweetsSearchRecentQueryParameters
+    ) -> Generator[GetV2TweetsSearchRecentResponseBody, None, None]:
         """
         ツイートの一覧を検索する。
 
         ページングされた API のレスポンスをイテレータで返す。
 
-        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-all
+        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-recent
         """
-        return get_paging_response_iter_sync(self.get, query)
+        return get_paging_response_body_iter_sync(self.get, query, "next_token")
 
-    def get_collected_response(
-        self, query: GetV2TweetsSearchAllQueryParameters
-    ) -> GetV2TweetsSearchAllResponseBody:
+    def get_collected_paging_response_body(
+        self, query: GetV2TweetsSearchRecentQueryParameters
+    ) -> GetV2TweetsSearchRecentResponseBody:
         """
         ツイートの一覧を検索する。
 
         ページングされた API のレスポンスをまとめて一つのレスポンスとして返す。
 
-        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-all
+        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-recent
         """
-        return get_collected_paging_response_sync(self.get, query)
+        return get_collected_paging_response_body_sync(self.get, query, "next_token")
 
 
-class AsyncGetV2TweetsSearchAllResources(GetV2TweetsSearchAllResources):
+class AsyncGetV2TweetsSearchRecentResources(GetV2TweetsSearchRecentResources):
     async def get(
-        self, query: GetV2TweetsSearchAllQueryParameters
-    ) -> GetV2TweetsSearchAllResponseBody:
+        self, query: GetV2TweetsSearchRecentQueryParameters
+    ) -> GetV2TweetsSearchRecentResponseBody:
         return super().get(query)
 
-    async def get_paging_response_iter(
-        self, query: GetV2TweetsSearchAllQueryParameters
-    ) -> AsyncGenerator[GetV2TweetsSearchAllResponseBody, None]:
-        return get_paging_response_iter_async(self.get, query)
-
-    async def get_collected_response(
-        self, query: GetV2TweetsSearchAllQueryParameters
-    ) -> GetV2TweetsSearchAllResponseBody:
-        return await get_collected_paging_response_async(self.get, query)
+    async def get_paging_response_body_iter(
+        self, query: GetV2TweetsSearchRecentQueryParameters
+    ) -> AsyncGenerator[GetV2TweetsSearchRecentResponseBody, None]:
+        return get_paging_response_body_iter_async(self.get, query, "next_token")
+
+    async def get_collected_paging_response_body(
+        self, query: GetV2TweetsSearchRecentQueryParameters
+    ) -> GetV2TweetsSearchRecentResponseBody:
+        return await get_collected_paging_response_body_async(
+            self.get, query, "next_token"
+        )
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,133 +1,136 @@
 from datetime import datetime
 from typing import AsyncGenerator, Generator, Literal, NotRequired, Optional, TypedDict
+from urllib import parse
 
 from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_expansion import Expansion
+from twitter_api.api.types.pagination_token import PaginationToken
 from twitter_api.api.types.v2_media.media_field import MediaField
 from twitter_api.api.types.v2_place.place_field import PlaceField
 from twitter_api.api.types.v2_poll.poll_field import PollField
 from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_search_query import SearchQuery
+from twitter_api.api.types.v2_tweet.tweet_expansion import TweetExpansion
 from twitter_api.api.types.v2_tweet.tweet_field import TweetField
 from twitter_api.api.types.v2_tweet.tweet_id import TweetId
 from twitter_api.api.types.v2_tweet.tweet_response_body import TweetsSearchResponseBody
 from twitter_api.api.types.v2_user.user_field import UserField
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.paging import (
-    get_collected_paging_response_async,
-    get_collected_paging_response_sync,
-    get_paging_response_iter_async,
-    get_paging_response_iter_sync,
+    get_collected_paging_response_body_async,
+    get_collected_paging_response_body_sync,
+    get_paging_response_body_iter_async,
+    get_paging_response_body_iter_sync,
 )
-from twitter_api.utils.datetime import rfc3339
-from twitter_api.utils.functional import map_optional
+from twitter_api.utils._datetime import rfc3339
+from twitter_api.utils._functional import map_optional
 
-ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets/search/recent")
+ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets/search/all")
 
-GetV2TweetsSearchRecentQueryParameters = TypedDict(
-    "GetV2TweetsSearchRecentQueryParameters",
+GetV2TweetsSearchAllQueryParameters = TypedDict(
+    "GetV2TweetsSearchAllQueryParameters",
     {
-        "query": str | SearchQuery,
+        "query": str,
         "start_time": NotRequired[Optional[datetime]],
         "end_time": NotRequired[Optional[datetime]],
         "since_id": NotRequired[Optional[TweetId]],
         "until_id": NotRequired[Optional[TweetId]],
         "sort_order": NotRequired[Optional[Literal["recency", "relevancy"]]],
-        "next_token": NotRequired[Optional[str]],
+        "next_token": NotRequired[Optional[PaginationToken]],
         "max_results": NotRequired[Optional[int]],
-        "expansions": NotRequired[Optional[CommaSeparatable[Expansion]]],
+        "expansions": NotRequired[Optional[CommaSeparatable[TweetExpansion]]],
         "place.fields": NotRequired[Optional[CommaSeparatable[PlaceField]]],
         "media.fields": NotRequired[Optional[CommaSeparatable[MediaField]]],
         "poll.fields": NotRequired[Optional[CommaSeparatable[PollField]]],
         "tweet.fields": NotRequired[Optional[CommaSeparatable[TweetField]]],
         "user.fields": NotRequired[Optional[CommaSeparatable[UserField]]],
     },
 )
 
 
-def _make_query(query: GetV2TweetsSearchRecentQueryParameters) -> dict:
+def _make_query(query: GetV2TweetsSearchAllQueryParameters) -> dict:
     return {
-        "query": str(query["query"]),
+        "query": parse.quote(str(query["query"])),
         "start_time": map_optional(rfc3339, query.get("start_time")),
         "end_time": map_optional(rfc3339, query.get("end_time")),
         "since_id": query.get("since_id"),
         "until_id": query.get("until_id"),
         "sort_order": query.get("sort_order"),
         "next_token": query.get("next_token"),
-        "max_results": query.get("max_results"),
+        "max_results": query.get("expansions"),
         "expansions": comma_separated_str(query.get("expansions")),
-        "place.fields": comma_separated_str(query.get("place.fields")),
-        "media.fields": comma_separated_str(query.get("media.fields")),
-        "poll.fields": comma_separated_str(query.get("poll.fields")),
+        "place.fields": query.get("place.fields"),
+        "media.fields": query.get("media.fields"),
+        "poll.fields": query.get("poll.fields"),
         "tweet.fields": comma_separated_str(query.get("tweet.fields")),
         "user.fields": comma_separated_str(query.get("user.fields")),
     }
 
 
-class GetV2TweetsSearchRecentResponseBody(TweetsSearchResponseBody):
+class GetV2TweetsSearchAllResponseBody(TweetsSearchResponseBody):
     pass
 
 
-class GetV2TweetsSearchRecentResources(ApiResources):
+class GetV2TweetsSearchAllResources(ApiResources):
     @oauth2_scopes(
         "tweet.read",
         "users.read",
     )
-    @rate_limit(ENDPOINT, "app", requests=450, mins=15)
-    @rate_limit(ENDPOINT, "user", requests=180, mins=15)
+    @rate_limit(ENDPOINT, "app", requests=300, mins=15)
+    @rate_limit(ENDPOINT, "app", requests=1, seconds=1)
     def get(
-        self, query: GetV2TweetsSearchRecentQueryParameters
-    ) -> GetV2TweetsSearchRecentResponseBody:
+        self, query: GetV2TweetsSearchAllQueryParameters
+    ) -> GetV2TweetsSearchAllResponseBody:
         """
         ツイートの一覧を検索する。
 
-        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-recent
+        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-all
         """
         return self.request_client.get(
             endpoint=ENDPOINT,
-            response_type=GetV2TweetsSearchRecentResponseBody,
+            response_body_type=GetV2TweetsSearchAllResponseBody,
             query=_make_query(query) if query is not None else None,
         )
 
-    def get_paging_response_iter(
-        self, query: GetV2TweetsSearchRecentQueryParameters
-    ) -> Generator[GetV2TweetsSearchRecentResponseBody, None, None]:
+    def get_paging_response_body_iter(
+        self, query: GetV2TweetsSearchAllQueryParameters
+    ) -> Generator[GetV2TweetsSearchAllResponseBody, None, None]:
         """
         ツイートの一覧を検索する。
 
         ページングされた API のレスポンスをイテレータで返す。
 
-        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-recent
+        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-all
         """
-        return get_paging_response_iter_sync(self.get, query)
+        return get_paging_response_body_iter_sync(self.get, query, "next_token")
 
-    def get_collected_response(
-        self, query: GetV2TweetsSearchRecentQueryParameters
-    ) -> GetV2TweetsSearchRecentResponseBody:
+    def get_collected_paging_response_body(
+        self, query: GetV2TweetsSearchAllQueryParameters
+    ) -> GetV2TweetsSearchAllResponseBody:
         """
         ツイートの一覧を検索する。
 
         ページングされた API のレスポンスをまとめて一つのレスポンスとして返す。
 
-        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-recent
+        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-all
         """
-        return get_collected_paging_response_sync(self.get, query)
+        return get_collected_paging_response_body_sync(self.get, query, "next_token")
 
 
-class AsyncGetV2TweetsSearchRecentResources(GetV2TweetsSearchRecentResources):
+class AsyncGetV2TweetsSearchAllResources(GetV2TweetsSearchAllResources):
     async def get(
-        self, query: GetV2TweetsSearchRecentQueryParameters
-    ) -> GetV2TweetsSearchRecentResponseBody:
+        self, query: GetV2TweetsSearchAllQueryParameters
+    ) -> GetV2TweetsSearchAllResponseBody:
         return super().get(query)
 
-    async def get_paging_response_iter(
-        self, query: GetV2TweetsSearchRecentQueryParameters
-    ) -> AsyncGenerator[GetV2TweetsSearchRecentResponseBody, None]:
-        return get_paging_response_iter_async(self.get, query)
-
-    async def get_collected_response(
-        self, query: GetV2TweetsSearchRecentQueryParameters
-    ) -> GetV2TweetsSearchRecentResponseBody:
-        return await get_collected_paging_response_async(self.get, query)
+    async def get_paging_response_body_iter(
+        self, query: GetV2TweetsSearchAllQueryParameters
+    ) -> AsyncGenerator[GetV2TweetsSearchAllResponseBody, None]:
+        return get_paging_response_body_iter_async(self.get, query, "next_token")
+
+    async def get_collected_paging_response_body(
+        self, query: GetV2TweetsSearchAllQueryParameters
+    ) -> GetV2TweetsSearchAllResponseBody:
+        return await get_collected_paging_response_body_async(
+            self.get, query, "next_token"
+        )
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 from datetime import datetime
-from typing import AsyncGenerator, Generator, NotRequired, Optional, TypedDict
+from typing import NotRequired, Optional, TypedDict
 
 from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_expansion import Expansion
 from twitter_api.api.types.v2_media.media_field import MediaField
 from twitter_api.api.types.v2_place.place_field import PlaceField
 from twitter_api.api.types.v2_poll.poll_field import PollField
 from twitter_api.api.types.v2_scope import oauth2_scopes
+from twitter_api.api.types.v2_tweet.tweet_expansion import TweetExpansion
 from twitter_api.api.types.v2_tweet.tweet_field import TweetField
 from twitter_api.api.types.v2_tweet.tweet_response_body import TweetsSearchResponseBody
 from twitter_api.api.types.v2_user.user_field import UserField
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
-from twitter_api.types.paging import (
-    get_collected_paging_response_async,
-    get_collected_paging_response_sync,
-    get_paging_response_iter_async,
-    get_paging_response_iter_sync,
-)
-from twitter_api.utils.datetime import rfc3339
-from twitter_api.utils.functional import map_optional
+from twitter_api.utils._datetime import rfc3339
+from twitter_api.utils._functional import map_optional
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets/search/stream")
 
 GetV2TweetsSearchStreamQueryParameters = TypedDict(
     "GetV2TweetsSearchStreamQueryParameters",
     {
         "backfill_minutes": NotRequired[Optional[int]],
         "start_time": NotRequired[Optional[datetime]],
         "end_time": NotRequired[Optional[datetime]],
-        "expansions": NotRequired[Optional[CommaSeparatable[Expansion]]],
+        "expansions": NotRequired[Optional[CommaSeparatable[TweetExpansion]]],
         "place.fields": NotRequired[Optional[CommaSeparatable[PlaceField]]],
         "media.fields": NotRequired[Optional[CommaSeparatable[MediaField]]],
         "poll.fields": NotRequired[Optional[CommaSeparatable[PollField]]],
         "tweet.fields": NotRequired[Optional[CommaSeparatable[TweetField]]],
         "user.fields": NotRequired[Optional[CommaSeparatable[UserField]]],
     },
 )
@@ -70,51 +64,17 @@
         """
         ツイートの一覧を検索する。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/filtered-stream/api-reference/get-tweets-search-stream
         """
         return self.request_client.get(
             endpoint=ENDPOINT,
-            response_type=GetV2TweetsSearchStreamResponseBody,
+            response_body_type=GetV2TweetsSearchStreamResponseBody,
             query=_make_query(query) if query is not None else None,
         )
 
-    def get_paging_response_iter(
-        self, query: Optional[GetV2TweetsSearchStreamQueryParameters] = None
-    ) -> Generator[GetV2TweetsSearchStreamResponseBody, None, None]:
-        """
-        ツイートの一覧を検索する。
-
-        ページングされた API のレスポンスをイテレータで返す。
-
-        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/filtered-stream/api-reference/get-tweets-search-stream
-        """
-        return get_paging_response_iter_sync(self.get, query)
-
-    def get_collected_response(
-        self, query: Optional[GetV2TweetsSearchStreamQueryParameters] = None
-    ) -> GetV2TweetsSearchStreamResponseBody:
-        """
-        ツイートの一覧を検索する。
-
-        ページングされた API のレスポンスをまとめて一つのレスポンスとして返す。
-
-        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/filtered-stream/api-reference/get-tweets-search-stream
-        """
-        return get_collected_paging_response_sync(self.get, query)
-
 
 class AsyncGetV2TweetsSearchStreamResources(GetV2TweetsSearchStreamResources):
     async def get(
         self, query: Optional[GetV2TweetsSearchStreamQueryParameters] = None
     ) -> GetV2TweetsSearchStreamResponseBody:
         return super().get(query)
-
-    async def get_paging_response_iter(
-        self, query: Optional[GetV2TweetsSearchStreamQueryParameters] = None
-    ) -> AsyncGenerator[GetV2TweetsSearchStreamResponseBody, None]:
-        return get_paging_response_iter_async(self.get, query)
-
-    async def get_collected_response(
-        self, query: Optional[GetV2TweetsSearchStreamQueryParameters] = None
-    ) -> GetV2TweetsSearchStreamResponseBody:
-        return await get_collected_paging_response_async(self.get, query)
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets_search_stream_rules/__init__.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         """
         ツイートの一覧を検索するフィルターの一覧を取得する。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/filtered-stream/api-reference/get-tweets-search-stream-rules
         """
         return self.request_client.post(
             endpoint=ENDPOINT,
-            response_type=GetV2TweetsSearchStreamRulesResponseBody,
+            response_body_type=GetV2TweetsSearchStreamRulesResponseBody,
             query=downcast_dict(query),
         )
 
 
 class AsyncGetV2TweetsSearchStreamRulesResources(GetV2TweetsSearchStreamRulesResources):
     async def get(
         self,
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         """
         ツイートの一覧を検索するフィルターを作成する。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/filtered-stream/api-reference/post-tweets-search-stream-rules
         """
         return self.request_client.post(
             endpoint=ENDPOINT,
-            response_type=PostV2TweetsSearchStreamRulesResponseBody,
+            response_body_type=PostV2TweetsSearchStreamRulesResponseBody,
             query=downcast_dict(query),
             body=downcast_dict(request_body),
         )
 
 
 class AsyncPostV2TweetsSearchStreamRulesResources(
     PostV2TweetsSearchStreamRulesResources
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_user/get_v2_user.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_user/get_v2_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from typing import NotRequired, Optional, TypedDict
 
 from pydantic import Field
 
 from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_expansion import Expansion
 from twitter_api.api.types.v2_scope import oauth2_scopes
 from twitter_api.api.types.v2_tweet.tweet import Tweet
 from twitter_api.api.types.v2_tweet.tweet_field import TweetField
 from twitter_api.api.types.v2_user.user import User
+from twitter_api.api.types.v2_user.user_expantion import UserExpansion
 from twitter_api.api.types.v2_user.user_field import UserField
 from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/users/:id")
 
 GetV2UserQueryParameters = TypedDict(
     "GetV2UserQueryParameters",
     {
-        "expansions": NotRequired[Optional[CommaSeparatable[Expansion]]],
+        "expansions": NotRequired[Optional[CommaSeparatable[UserExpansion]]],
         "tweet.fields": NotRequired[Optional[CommaSeparatable[TweetField]]],
         "user.fields": NotRequired[Optional[CommaSeparatable[UserField]]],
     },
 )
 
 
 def _make_query(query: GetV2UserQueryParameters) -> dict:
@@ -62,15 +62,15 @@
 
         refer: https://developer.twitter.com/en/docs/twitter-api/users/lookup/api-reference/get-users-id
         """
         return self.request_client.get(
             endpoint=ENDPOINT,
             url=ENDPOINT.url.replace(":id", id),
             query=_make_query(query) if query is not None else None,
-            response_type=GetV2UserResponseBody,
+            response_body_type=GetV2UserResponseBody,
         )
 
 
 class AsyncGetV2UserResources(GetV2UserResources):
     async def get(
         self,
         id: UserId,
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_user_followers/get_v2_user_followers.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_followers/get_v2_user_followers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from functools import partial
 from typing import AsyncGenerator, Generator, NotRequired, Optional, Self, TypedDict
 
 from pydantic import Field
 
 from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_expansion import Expansion
+from twitter_api.api.types.pagination_token import PaginationToken
 from twitter_api.api.types.v2_scope import oauth2_scopes
 from twitter_api.api.types.v2_tweet.tweet import Tweet
 from twitter_api.api.types.v2_tweet.tweet_field import TweetField
 from twitter_api.api.types.v2_user.user import User
+from twitter_api.api.types.v2_user.user_expantion import UserExpansion
 from twitter_api.api.types.v2_user.user_field import UserField
 from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.paging import (
     PageResponseBody,
-    get_collected_paging_response_async,
-    get_collected_paging_response_sync,
-    get_paging_response_iter_async,
-    get_paging_response_iter_sync,
+    get_collected_paging_response_body_async,
+    get_collected_paging_response_body_sync,
+    get_paging_response_body_iter_async,
+    get_paging_response_body_iter_sync,
 )
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/users/:id/followers")
 
 GetV2UserFollowersQueryParameters = TypedDict(
     "GetV2UserFollowersQueryParameters",
     {
-        "expansions": NotRequired[Optional[CommaSeparatable[Expansion]]],
+        "expansions": NotRequired[Optional[CommaSeparatable[UserExpansion]]],
         "pagination_token": NotRequired[Optional[str]],
         "max_results": NotRequired[Optional[int]],
         "tweet.fields": NotRequired[Optional[CommaSeparatable[TweetField]]],
         "user.fields": NotRequired[Optional[CommaSeparatable[UserField]]],
     },
 )
 
@@ -45,16 +46,16 @@
         "tweet.fields": comma_separated_str(query.get("tweet.fields")),
         "user.fields": comma_separated_str(query.get("user.fields")),
     }
 
 
 class GetV2UserFollowersResponseBodyMeta(ExtraPermissiveModel):
     result_count: int
-    next_token: Optional[str] = None
-    previous_token: Optional[str] = None
+    next_token: Optional[PaginationToken] = None
+    previous_token: Optional[PaginationToken] = None
 
     def extend(self, other: Self) -> None:
         self.result_count += other.result_count
         self.next_token = None
         self.previous_token = None
 
 
@@ -70,15 +71,15 @@
     meta: GetV2UserFollowersResponseBodyMeta
     includes: GetV2UserFollowersResponseBodyIncludes = Field(
         default_factory=GetV2UserFollowersResponseBodyIncludes,
     )
     errors: Optional[list[dict]] = None
 
     @property
-    def meta_next_token(self) -> str | None:
+    def meta_next_token(self) -> PaginationToken | None:
         return self.meta.next_token
 
     def extend(self, other: Self) -> None:
         self.data.extend(other.data)
         self.meta.extend(other.meta)
         self.includes.extend(other.includes)
 
@@ -107,60 +108,68 @@
 
         refer: https://developer.twitter.com/en/docs/twitter-api/users/follows/api-reference/get-users-id-followers
         """
         return self.request_client.get(
             endpoint=ENDPOINT,
             url=ENDPOINT.url.replace(":id", id),
             query=_make_query(query) if query is not None else None,
-            response_type=GetV2UserFollowersResponseBody,
+            response_body_type=GetV2UserFollowersResponseBody,
         )
 
-    def get_paging_response_iter(
+    def get_paging_response_body_iter(
         self,
         id: UserId,
         query: Optional[GetV2UserFollowersQueryParameters] = None,
     ) -> Generator[GetV2UserFollowersResponseBody, None, None]:
         """
         ユーザのフォロワーの一覧を取得する。
 
         ページングされた API のレスポンスをイテレータで返す。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/users/follows/api-reference/get-users-id-followers
         """
-        return get_paging_response_iter_sync(partial(self.get, id), query)
+        return get_paging_response_body_iter_sync(
+            partial(self.get, id), query, "pagination_token"
+        )
 
-    def get_collected_response(
+    def get_collected_paging_response_body(
         self,
         id: UserId,
         query: Optional[GetV2UserFollowersQueryParameters] = None,
     ) -> GetV2UserFollowersResponseBody:
         """
         ユーザのフォロワーの一覧を取得する。
 
         ページングされた API のレスポンスをまとめて一つのレスポンスとして返す。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/users/follows/api-reference/get-users-id-followers
         """
-        return get_collected_paging_response_sync(partial(self.get, id), query)
+        return get_collected_paging_response_body_sync(
+            partial(self.get, id), query, "pagination_token"
+        )
 
 
 class AsyncGetV2UserFollowersResources(GetV2UserFollowersResources):
     async def get(
         self,
         id: UserId,
         query: Optional[GetV2UserFollowersQueryParameters] = None,
     ) -> GetV2UserFollowersResponseBody:
         return super().get(id, query)
 
-    async def get_paging_response_iter(
+    async def get_paging_response_body_iter(
         self,
         id: UserId,
         query: Optional[GetV2UserFollowersQueryParameters] = None,
     ) -> AsyncGenerator[GetV2UserFollowersResponseBody, None]:
-        return get_paging_response_iter_async(partial(self.get, id), query)
+        return get_paging_response_body_iter_async(
+            partial(self.get, id), query, "pagination_token"
+        )
 
-    async def get_collected_response(
+    async def get_collected_paging_response_body(
         self,
         id: UserId,
         query: Optional[GetV2UserFollowersQueryParameters] = None,
     ) -> GetV2UserFollowersResponseBody:
-        return await get_collected_paging_response_async(partial(self.get, id), query)
+        return await get_collected_paging_response_body_async(
+            partial(self.get, id), query, "pagination_token"
+        )
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_user_following/post_v2_user_following.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_following/post_v2_user_following.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
         refer: https://developer.twitter.com/en/docs/twitter-api/users/follows/api-reference/post-users-source_user_id-following
         """
         return self.request_client.post(
             endpoint=ENDPOINT,
             url=ENDPOINT.url.replace(":id", id),
             body=downcast_dict(request_body),
-            response_type=PostV2UserFollowingResponseBody,
+            response_body_type=PostV2UserFollowingResponseBody,
         )
 
 
 class AsyncPostV2UserFollowingResources(PostV2UserFollowingResources):
     async def post(
         self,
         id: UserId,
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 from functools import partial
 from typing import AsyncGenerator, Generator, NotRequired, Optional, Self, TypedDict
 
 from pydantic import Field
 
 from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_expansion import Expansion
+from twitter_api.api.types.pagination_token import PaginationToken
 from twitter_api.api.types.v2_media.media import Media
 from twitter_api.api.types.v2_media.media_field import MediaField
 from twitter_api.api.types.v2_place.place import Place
 from twitter_api.api.types.v2_place.place_field import PlaceField
 from twitter_api.api.types.v2_poll.poll import Poll
 from twitter_api.api.types.v2_poll.poll_field import PollField
 from twitter_api.api.types.v2_scope import oauth2_scopes
 from twitter_api.api.types.v2_tweet.tweet import Tweet
 from twitter_api.api.types.v2_tweet.tweet_field import TweetField
 from twitter_api.api.types.v2_user.user import User
+from twitter_api.api.types.v2_user.user_expantion import UserExpansion
 from twitter_api.api.types.v2_user.user_field import UserField
 from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.paging import (
     PageResponseBody,
-    get_collected_paging_response_async,
-    get_collected_paging_response_sync,
-    get_paging_response_iter_async,
-    get_paging_response_iter_sync,
+    get_collected_paging_response_body_async,
+    get_collected_paging_response_body_sync,
+    get_paging_response_body_iter_async,
+    get_paging_response_body_iter_sync,
 )
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/users/:id/liked_tweets")
 
 GetV2UserLikedTweetsQueryParameters = TypedDict(
     "GetV2UserLikedTweetsQueryParameters",
     {
-        "expansions": NotRequired[Optional[CommaSeparatable[Expansion]]],
+        "expansions": NotRequired[Optional[CommaSeparatable[UserExpansion]]],
         "pagination_token": NotRequired[Optional[str]],
         "max_results": NotRequired[Optional[int]],
         "media.fields": NotRequired[Optional[CommaSeparatable[MediaField]]],
         "place.fields": NotRequired[Optional[CommaSeparatable[PlaceField]]],
         "poll.fields": NotRequired[Optional[CommaSeparatable[PollField]]],
         "tweet.fields": NotRequired[Optional[CommaSeparatable[TweetField]]],
         "user.fields": NotRequired[Optional[CommaSeparatable[UserField]]],
@@ -72,16 +73,16 @@
         self.places.extend(other.places)
         self.media.extend(other.media)
         self.polls.extend(other.polls)
 
 
 class GetV2UserLikedTweetsResponseBodyMeta(ExtraPermissiveModel):
     result_count: int
-    next_token: Optional[str] = None
-    previous_token: Optional[str] = None
+    next_token: Optional[PaginationToken] = None
+    previous_token: Optional[PaginationToken] = None
 
     def extend(self, other: Self) -> None:
         self.result_count += other.result_count
         self.next_token = None
         self.previous_token = None
 
 
@@ -90,15 +91,15 @@
     meta: Optional[GetV2UserLikedTweetsResponseBodyMeta] = None
     includes: GetV2UserLikedTweetsResponseBodyIncludes = Field(
         default_factory=GetV2UserLikedTweetsResponseBodyIncludes,
     )
     errors: Optional[list[dict]] = None
 
     @property
-    def meta_next_token(self) -> str | None:
+    def meta_next_token(self) -> PaginationToken | None:
         if self.meta is None:
             return None
 
         return self.meta.next_token
 
     def extend(self, other: Self) -> None:
         self.data.extend(other.data)
@@ -132,60 +133,68 @@
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/likes/api-reference/get-users-id-liked_tweets
         """
         return self.request_client.get(
             endpoint=ENDPOINT,
             url=ENDPOINT.url.replace(":id", id),
             query=_make_query(query) if query is not None else None,
-            response_type=GetV2UserLikedTweetsResponseBody,
+            response_body_type=GetV2UserLikedTweetsResponseBody,
         )
 
-    def get_paging_response_iter(
+    def get_paging_response_body_iter(
         self,
         id: UserId,
         query: Optional[GetV2UserLikedTweetsQueryParameters] = None,
     ) -> Generator[GetV2UserLikedTweetsResponseBody, None, None]:
         """
         ユーザが「いいね」をしているツイートの一覧を取得する。
 
         ページングされた API のレスポンスをイテレータで返す。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/likes/api-reference/get-users-id-liked_tweets
         """
-        return get_paging_response_iter_sync(partial(self.get, id), query)
+        return get_paging_response_body_iter_sync(
+            partial(self.get, id), query, "pagination_token"
+        )
 
-    def get_collected_response(
+    def get_collected_paging_response_body(
         self,
         id: UserId,
         query: Optional[GetV2UserLikedTweetsQueryParameters] = None,
     ) -> GetV2UserLikedTweetsResponseBody:
         """
         ユーザが「いいね」をしているツイートの一覧を取得する。
 
         ページングされた API のレスポンスをまとめて一つのレスポンスとして返す。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/likes/api-reference/get-users-id-liked_tweets
         """
-        return get_collected_paging_response_sync(partial(self.get, id), query)
+        return get_collected_paging_response_body_sync(
+            partial(self.get, id), query, "pagination_token"
+        )
 
 
 class AsyncGetV2UserLikedTweetsResources(GetV2UserLikedTweetsResources):
     async def get(
         self,
         id: UserId,
         query: Optional[GetV2UserLikedTweetsQueryParameters] = None,
     ) -> GetV2UserLikedTweetsResponseBody:
         return super().get(id, query)
 
-    async def get_paging_response_iter(
+    async def get_paging_response_body_iter(
         self,
         id: UserId,
         query: Optional[GetV2UserLikedTweetsQueryParameters] = None,
     ) -> AsyncGenerator[GetV2UserLikedTweetsResponseBody, None]:
-        return get_paging_response_iter_async(partial(self.get, id), query)
+        return get_paging_response_body_iter_async(
+            partial(self.get, id), query, "pagination_token"
+        )
 
-    async def get_collected_response(
+    async def get_collected_paging_response_body(
         self,
         id: UserId,
         query: Optional[GetV2UserLikedTweetsQueryParameters] = None,
     ) -> GetV2UserLikedTweetsResponseBody:
-        return await get_collected_paging_response_async(partial(self.get, id), query)
+        return await get_collected_paging_response_body_async(
+            partial(self.get, id), query, "pagination_token"
+        )
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_user_retweets/post_v2_user_retweets.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_retweets/post_v2_user_retweets.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/retweets/api-reference/post-users-id-retweets
         """
         return self.request_client.post(
             endpoint=ENDPOINT,
             url=ENDPOINT.url.replace(":id", id),
             body=downcast_dict(request_body),
-            response_type=PostV2UserRetweetsResponseBody,
+            response_body_type=PostV2UserRetweetsResponseBody,
         )
 
 
 class AsyncPostV2UserRetweetsResources(PostV2UserRetweetsResources):
     async def post(
         self,
         id: UserId,
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_user_tweets/get_v2_user_tweets.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_tweets/get_v2_user_tweets.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,53 +9,54 @@
     Self,
     TypedDict,
 )
 
 from pydantic import Field
 
 from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_expansion import Expansion
+from twitter_api.api.types.pagination_token import PaginationToken
 from twitter_api.api.types.v2_media.media import Media
 from twitter_api.api.types.v2_media.media_field import MediaField
 from twitter_api.api.types.v2_place.place import Place
 from twitter_api.api.types.v2_place.place_field import PlaceField
 from twitter_api.api.types.v2_poll.poll import Poll
 from twitter_api.api.types.v2_poll.poll_field import PollField
 from twitter_api.api.types.v2_scope import oauth2_scopes
 from twitter_api.api.types.v2_tweet.tweet import Tweet
 from twitter_api.api.types.v2_tweet.tweet_field import TweetField
 from twitter_api.api.types.v2_tweet.tweet_id import TweetId
 from twitter_api.api.types.v2_user.user import User
+from twitter_api.api.types.v2_user.user_expantion import UserExpansion
 from twitter_api.api.types.v2_user.user_field import UserField
 from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.paging import (
     PageResponseBody,
-    get_collected_paging_response_async,
-    get_collected_paging_response_sync,
-    get_paging_response_iter_async,
-    get_paging_response_iter_sync,
+    get_collected_paging_response_body_async,
+    get_collected_paging_response_body_sync,
+    get_paging_response_body_iter_async,
+    get_paging_response_body_iter_sync,
 )
-from twitter_api.utils.datetime import rfc3339
-from twitter_api.utils.functional import map_optional
+from twitter_api.utils._datetime import rfc3339
+from twitter_api.utils._functional import map_optional
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/users/:id/tweets")
 
 GetV2UserTweetsQueryParameters = TypedDict(
     "GetV2UserTweetsQueryParameters",
     {
         "start_time": NotRequired[Optional[datetime]],
         "end_time": NotRequired[Optional[datetime]],
         "since_id": NotRequired[Optional[TweetId]],
         "until_id": NotRequired[Optional[TweetId]],
         "exclude": NotRequired[Optional[Literal["retweets", "replies"]]],
-        "expansions": NotRequired[Optional[CommaSeparatable[Expansion]]],
+        "expansions": NotRequired[Optional[CommaSeparatable[UserExpansion]]],
         "pagination_token": NotRequired[Optional[str]],
         "max_results": NotRequired[Optional[int]],
         "media.fields": NotRequired[Optional[CommaSeparatable[MediaField]]],
         "place.fields": NotRequired[Optional[CommaSeparatable[PlaceField]]],
         "poll.fields": NotRequired[Optional[CommaSeparatable[PollField]]],
         "tweet.fields": NotRequired[Optional[CommaSeparatable[TweetField]]],
         "user.fields": NotRequired[Optional[CommaSeparatable[UserField]]],
@@ -96,16 +97,16 @@
         self.polls.extend(other.polls)
 
 
 class GetV2UserTweetsResponseBodyMeta(ExtraPermissiveModel):
     result_count: int
     oldest_id: TweetId
     newest_id: TweetId
-    next_token: Optional[str] = None
-    previous_token: Optional[str] = None
+    next_token: Optional[PaginationToken] = None
+    previous_token: Optional[PaginationToken] = None
 
     def extend(self, other: Self) -> None:
         self.result_count += other.result_count
         self.next_token = None
         self.previous_token = None
 
 
@@ -114,15 +115,15 @@
     includes: GetV2UserTweetsResponseBodyIncludes = Field(
         default_factory=GetV2UserTweetsResponseBodyIncludes,
     )
     meta: GetV2UserTweetsResponseBodyMeta
     errors: Optional[list[dict]] = None
 
     @property
-    def meta_next_token(self) -> str | None:
+    def meta_next_token(self) -> PaginationToken | None:
         return self.meta.next_token
 
     def extend(self, other: Self) -> None:
         self.data.extend(other.data)
         self.meta.extend(other.meta)
         self.includes.extend(other.includes)
 
@@ -150,60 +151,68 @@
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/timelines/api-reference/get-users-id-tweets
         """
         return self.request_client.get(
             endpoint=ENDPOINT,
             url=ENDPOINT.url.replace(":id", id),
             query=_make_query(query) if query is not None else None,
-            response_type=GetV2UserTweetsResponseBody,
+            response_body_type=GetV2UserTweetsResponseBody,
         )
 
-    def get_paging_response_iter(
+    def get_paging_response_body_iter(
         self,
         id: UserId,
         query: Optional[GetV2UserTweetsQueryParameters] = None,
     ) -> Generator[GetV2UserTweetsResponseBody, None, None]:
         """
         ユーザのツイートの一覧を取得する。
 
         ページングされた API のレスポンスをイテレータで返す。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/timelines/api-reference/get-users-id-tweets
         """
-        return get_paging_response_iter_sync(partial(self.get, id), query)
+        return get_paging_response_body_iter_sync(
+            partial(self.get, id), query, "pagination_token"
+        )
 
-    def get_collected_response(
+    def get_collected_paging_response_body(
         self,
         id: UserId,
         query: Optional[GetV2UserTweetsQueryParameters] = None,
     ) -> GetV2UserTweetsResponseBody:
         """
         ユーザのツイートの一覧を取得する。
 
         ページングされた API のレスポンスをまとめて一つのレスポンスとして返す。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/timelines/api-reference/get-users-id-tweets
         """
-        return get_collected_paging_response_sync(partial(self.get, id), query)
+        return get_collected_paging_response_body_sync(
+            partial(self.get, id), query, "pagination_token"
+        )
 
 
 class AsyncGetV2UserTweetsResources(GetV2UserTweetsResources):
     async def get(
         self,
         id: UserId,
         query: Optional[GetV2UserTweetsQueryParameters] = None,
     ) -> GetV2UserTweetsResponseBody:
         return super().get(id, query)
 
-    async def get_paging_response_iter(
+    async def get_paging_response_body_iter(
         self,
         id: UserId,
         query: Optional[GetV2UserTweetsQueryParameters] = None,
     ) -> AsyncGenerator[GetV2UserTweetsResponseBody, None]:
-        return get_paging_response_iter_async(partial(self.get, id), query)
+        return get_paging_response_body_iter_async(
+            partial(self.get, id), query, "pagination_token"
+        )
 
-    async def get_collected_response(
+    async def get_collected_paging_response_body(
         self,
         id: UserId,
         query: Optional[GetV2UserTweetsQueryParameters] = None,
     ) -> GetV2UserTweetsResponseBody:
-        return await get_collected_paging_response_async(partial(self.get, id), query)
+        return await get_collected_paging_response_body_async(
+            partial(self.get, id), query, "pagination_token"
+        )
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/resources/v2_users/get_v2_users.py` & `twitter_api_py-0.2.0/twitter_api/api/resources/v2_users/get_v2_users.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from typing import NotRequired, Optional, TypedDict
 
 from pydantic import Field
 
 from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_expansion import Expansion
 from twitter_api.api.types.v2_scope import oauth2_scopes
 from twitter_api.api.types.v2_tweet.tweet import Tweet
 from twitter_api.api.types.v2_tweet.tweet_field import TweetField
 from twitter_api.api.types.v2_user.user import User
+from twitter_api.api.types.v2_user.user_expantion import UserExpansion
 from twitter_api.api.types.v2_user.user_field import UserField
 from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/users")
 
 GetV2UsersQueryParameters = TypedDict(
     "GetV2UsersQueryParameters",
     {
         "ids": CommaSeparatable[UserId],
-        "expansions": NotRequired[Optional[CommaSeparatable[Expansion]]],
+        "expansions": NotRequired[Optional[CommaSeparatable[UserExpansion]]],
         "tweet.fields": NotRequired[Optional[CommaSeparatable[TweetField]]],
         "user.fields": NotRequired[Optional[CommaSeparatable[UserField]]],
     },
 )
 
 
 def _make_query(query: GetV2UsersQueryParameters) -> dict:
@@ -59,14 +59,14 @@
         ユーザの一覧を取得する。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/users/lookup/api-reference/get-users
         """
         return self.request_client.get(
             endpoint=ENDPOINT,
             query=_make_query(query),
-            response_type=GetV2UsersResponseBody,
+            response_body_type=GetV2UsersResponseBody,
         )
 
 
 class AsyncGetV2UsersResources(GetV2UsersResources):
     async def get(self, query: GetV2UsersQueryParameters) -> GetV2UsersResponseBody:
         return super().get(query)
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/oauth1/oauth1_access_token.py` & `twitter_api_py-0.2.0/twitter_api/api/types/oauth1/oauth1_access_token.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from typing_extensions import Literal
+from typing import Generic
 
-from twitter_api.api.types.v2_scope import Scope
 from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.client.oauth_session.twitter_oauth1_session import TwitterOAuth1Session
 from twitter_api.types.chainable import Chainable
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.generic_client import TwitterApiGenericClient
 from twitter_api.types.oauth import AccessSecret, AccessToken
 
 
-class OAuth1AccessToken(Chainable, ExtraPermissiveModel):
+class OAuth1AccessToken(
+    Chainable, ExtraPermissiveModel, Generic[TwitterApiGenericClient]
+):
     oauth_token: AccessToken
     oauth_token_secret: AccessSecret
     user_id: UserId
     screen_name: str
-    _session: TwitterOAuth1Session
+    _session: TwitterOAuth1Session[TwitterApiGenericClient]
 
-    def generate_client(self):
+    def generate_client(self) -> TwitterApiGenericClient:
         return self._session.generate_client(self.oauth_token, self.oauth_token_secret)
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/oauth1/oauth1_authorization.py` & `twitter_api_py-0.2.0/twitter_api/api/types/oauth1/oauth1_authorization.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import sys
 from textwrap import dedent
-from typing import Callable, Optional, Self, TextIO
+from typing import Callable, Generic, Optional, Self, TextIO
 
 from twitter_api.client.oauth_session.twitter_oauth1_session import TwitterOAuth1Session
 from twitter_api.types.chainable import Chainable
+from twitter_api.types.generic_client import TwitterApiGenericClient
 from twitter_api.types.http import Url
 
 
-class OAuth1Authorization(Chainable):
+class OAuth1Authorization(Chainable, Generic[TwitterApiGenericClient]):
     def __init__(
         self,
         authorization_url: Url,
-        session: TwitterOAuth1Session,
+        session: TwitterOAuth1Session[TwitterApiGenericClient],
     ) -> None:
         self.authorization_url = authorization_url
         self._session = session
 
     def open_request_url(self) -> Self:
         """
         ブラウザで認証画面を開く。
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/oauth2/oauth2_authorization.py` & `twitter_api_py-0.2.0/twitter_api/api/types/oauth2/oauth2_authorization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import sys
 from textwrap import dedent
-from typing import Callable, Optional, Self, TextIO
+from typing import Callable, Generic, Optional, Self, TextIO
 
 from twitter_api.client.oauth_session.twitter_oauth2_session import TwitterOAuth2Session
 from twitter_api.types.chainable import Chainable
+from twitter_api.types.generic_client import TwitterApiGenericClient
 from twitter_api.types.http import Url
 
 
-class OAuth2Authorization(Chainable):
+class OAuth2Authorization(Chainable, Generic[TwitterApiGenericClient]):
     def __init__(
         self,
         authorization_url: Url,
         state: str,
         code_verifier: str,
-        session: TwitterOAuth2Session,
+        session: TwitterOAuth2Session[TwitterApiGenericClient],
     ) -> None:
         self.authorization_url = authorization_url
         self.state = state
         self.code_verifier = code_verifier
         self._session = session
 
     def open_request_url(self) -> Self:
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/v2_dm_conversation/dm_conversation_message.py` & `twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_conversation/dm_conversation_message.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/v2_expansion.py` & `twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_expansion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Literal, TypeAlias
 
-Expansion: TypeAlias = Literal[
+TweetExpansion: TypeAlias = Literal[
     "attachments.poll_ids",
     "attachments.media_keys",
     "author_id",
     "edit_history_tweet_ids",
     "entities.mentions.username",
     "geo.place_id",
     "in_reply_to_user_id",
     "referenced_tweets.id",
     "referenced_tweets.id.author_id",
 ]
 
-ALL_EXPANSIONS: list[Expansion] = [
+ALL_TWEET_EXPANSIONS: list[TweetExpansion] = [
     "attachments.poll_ids",
     "attachments.media_keys",
     "author_id",
     "edit_history_tweet_ids",
     "entities.mentions.username",
     "geo.place_id",
     "in_reply_to_user_id",
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/v2_media/media.py` & `twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/v2_media/media_field.py` & `twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/v2_place/place.py` & `twitter_api_py-0.2.0/twitter_api/api/types/v2_place/place.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/v2_poll/poll.py` & `twitter_api_py-0.2.0/twitter_api/api/types/v2_poll/poll.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/v2_retweet/retweet.py` & `twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/v2_retweet/retweet_entities_description.py` & `twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_entities_description.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/v2_scope.py` & `twitter_api_py-0.2.0/twitter_api/api/types/v2_scope.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet.py` & `twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_entities.py` & `twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_entities.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_field.py` & `twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/v2_tweet/tweet_response_body.py` & `twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_response_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from abc import ABCMeta, abstractmethod
 from typing import Optional, Self
 
 from pydantic import Field
 
+from twitter_api.api.types.pagination_token import PaginationToken
 from twitter_api.api.types.v2_media.media import Media
 from twitter_api.api.types.v2_place.place import Place
 from twitter_api.api.types.v2_poll.poll import Poll
 from twitter_api.api.types.v2_tweet.tweet import Tweet
 from twitter_api.api.types.v2_tweet.tweet_id import TweetId
 from twitter_api.api.types.v2_user.user import User
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
@@ -171,16 +172,16 @@
         return None
 
 
 class TweetsResponseBodyMeta(ExtraPermissiveModel):
     result_count: int
     newest_id: Optional[TweetId] = None
     oldest_id: Optional[TweetId] = None
-    next_token: Optional[str] = None
-    previous_token: Optional[str] = None
+    next_token: Optional[PaginationToken] = None
+    previous_token: Optional[PaginationToken] = None
 
     def extend(self, other: Self) -> None:
         self.result_count += other.result_count
 
         if self.newest_id is not None and other.newest_id is not None:
             if int(self.newest_id) < int(other.newest_id):
                 self.newest_id = other.newest_id
@@ -201,15 +202,15 @@
     meta: TweetsResponseBodyMeta
 
 
 class TweetsSearchResponseBody(
     TweetsResponseBody, _TweetsSearchResponseBody, PageResponseBody
 ):
     @property
-    def meta_next_token(self) -> str | None:
+    def meta_next_token(self) -> PaginationToken | None:
         return self.meta.next_token
 
     def extend(self, other: Self) -> None:
         self.data.extend(other.data)
         self.includes.extend(other.includes)
         self.meta.extend(other.meta)
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/v2_user/user.py` & `twitter_api_py-0.2.0/twitter_api/api/types/v2_user/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime
 from typing import Any, Optional
 
+from twitter_api.api.types.v2_user.user_verified_type import UserVerifiedType
 from twitter_api.api.types.v2_user.username import Username
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.http import Url
 
 from ..v2_tweet.tweet_id import TweetId
 from .user_id import UserId
 
@@ -19,8 +20,9 @@
     location: Optional[str] = None
     pinned_tweet_id: Optional[TweetId] = None
     profile_image_url: Optional[Url] = None
     protected: Optional[bool] = None
     public_metrics: Optional[dict[str, Any]] = None
     url: Optional[Url] = None
     verified: Optional[bool] = None
+    verified_type: Optional[UserVerifiedType] = None
     withheld: Optional[dict[str, Any]] = None
```

### Comparing `twitter_api_py-0.1.0/twitter_api/api/types/v2_user/user_field.py` & `twitter_api_py-0.2.0/twitter_api/api/types/v2_user/user_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.1.0/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py` & `twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,20 @@
-from twitter_api.client.oauth_session.resources.oauth1_authenticate import (
-    OAuth1AuthenticateSessionResources,
-    OauthAuth1enticateUrl,
+from twitter_api.client.oauth_flow.twitter_oauth1_authorization_client import (
+    TwitterOAuth1AuthorizeClient,
 )
-from twitter_api.client.oauth_session.resources.oauth1_authorize import (
-    OAuth1AuthorizeSessionResources,
-    Oauth1AuthorizeUrl,
+from twitter_api.client.oauth_session.resources.session_resources import (
+    OAuth1SessionResources,
 )
-from twitter_api.client.oauth_session.twitter_oauth1_session import TwitterOAuth1Session
-from twitter_api.error import NeverError
-from twitter_api.types.chainable import Chainable
+from twitter_api.types.generic_client import TwitterApiGenericClient
 
 
-class TwitterOAuth1AuthorizeClient(Chainable):
-    def __init__(self, session: TwitterOAuth1Session) -> None:
-        self._session = session
+class PostOAuth1RequestTokenSessionResources(
+    OAuth1SessionResources[TwitterApiGenericClient]
+):
+    def post(self) -> TwitterOAuth1AuthorizeClient[TwitterApiGenericClient]:
+        """
+        OAuth 1.0a の最初のステップ。
+        ユーザーアクセストークンのセットを生成するためにリクエストを送信する。
 
-    def resource(
-        self, url: OauthAuth1enticateUrl | Oauth1AuthorizeUrl
-    ) -> OAuth1AuthenticateSessionResources | OAuth1AuthorizeSessionResources:
-        if url == "https://api.twitter.com/oauth/authenticate":
-            return OAuth1AuthenticateSessionResources(
-                self._session,
-            )
-        elif url == "https://api.twitter.com/oauth/authorize":
-            return OAuth1AuthorizeSessionResources(
-                self._session,
-            )
-        else:
-            raise NeverError(url)
+        refer: https://developer.twitter.com/en/docs/authentication/api-reference/request_token
+        """
+        return self._session.request_token()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `twitter_api_py-0.1.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py` & `twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+from typing import Generic
+
 from twitter_api.client.oauth_session.resources.oauth1_request_token import (
     OAuth1RequestTokenSessionResources,
     Oauth1RequestTokenUrl,
 )
 from twitter_api.client.oauth_session.twitter_oauth1_session import TwitterOAuth1Session
 from twitter_api.types.chainable import Chainable
+from twitter_api.types.generic_client import TwitterApiGenericClient
 
 
-class TwitterOAuth1RequestTokenClient(Chainable):
-    def __init__(self, session: TwitterOAuth1Session) -> None:
+class TwitterOAuth1RequestTokenClient(Chainable, Generic[TwitterApiGenericClient]):
+    def __init__(self, session: TwitterOAuth1Session[TwitterApiGenericClient]) -> None:
         self._session = session
 
-    def resource(
+    def request(
         self, url: Oauth1RequestTokenUrl
-    ) -> OAuth1RequestTokenSessionResources:
+    ) -> OAuth1RequestTokenSessionResources[TwitterApiGenericClient]:
         return OAuth1RequestTokenSessionResources(
             self._session,
         )
```

### Comparing `twitter_api_py-0.1.0/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py` & `twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,87 +1,57 @@
-import os
-from typing import Optional
+from typing import Callable
 
-from twitter_api.client.oauth_session.resources.v2_oauth2_token import (
-    V2OAuth2TokenRerources,
-    V2Oauth2TokenUrl,
+from twitter_api.client.oauth_flow.twitter_oauth1_authorization_client import (
+    TwitterOAuth1AuthorizeClient,
 )
-from twitter_api.client.oauth_session.twitter_oauth2_real_session import (
-    TwitterOAuth2RealSession,
+from twitter_api.client.oauth_session.resources.oauth1_authenticate import (
+    OauthAuth1enticateUrl,
 )
-from twitter_api.client.oauth_session.twitter_oauth2_session import TwitterOAuth2Session
-from twitter_api.types.chainable import Chainable
-from twitter_api.types.oauth import CallbackUrl, ClientId, ClientSecret, Env
+from twitter_api.client.oauth_session.resources.oauth1_authorize import (
+    Oauth1AuthorizeUrl,
+)
+from twitter_api.client.oauth_session.twitter_oauth1_session import TwitterOAuth1Session
+from twitter_api.types.generic_client import TwitterApiGenericMockClient
+from twitter_api.types.oauth import AccessSecret, AccessToken, CallbackUrl
 
 
-class TwitterOAuth2AccessTokenClient(Chainable):
+class TwitterOAuth1MockSession(TwitterOAuth1Session[TwitterApiGenericMockClient]):
     def __init__(
         self,
-        authorization_response_url: CallbackUrl,
-        state: str,
-        code_verifier: str,
-        session: TwitterOAuth2Session,
-    ):
-        self.authorization_response_url = authorization_response_url
-        self.state = state
-        self.code_verifier = code_verifier
-        self._session = session
-
-    def resource(self, url: V2Oauth2TokenUrl):
-        return V2OAuth2TokenRerources(
-            authorization_response_url=self.authorization_response_url,
-            state=self.state,
-            code_verifier=self.code_verifier,
-            session=self._session,
-        )
+        client_generator: Callable[
+            [AccessToken, AccessSecret], TwitterApiGenericMockClient
+        ],
+    ) -> None:
+        self._client_generator = client_generator
 
-    @classmethod
-    def from_authorization_response_url(
-        cls,
-        *,
-        client_id: ClientId,
-        client_secret: ClientSecret,
-        callback_url: CallbackUrl,
-        authorization_response_url: CallbackUrl,
-        state: str,
-        code_verifier: str,
+    def request_token(self) -> TwitterOAuth1AuthorizeClient:
+        return TwitterOAuth1AuthorizeClient(session=self)
+
+    def generate_authorization_url(
+        self,
+        url: OauthAuth1enticateUrl | Oauth1AuthorizeUrl,
     ):
-        session = TwitterOAuth2RealSession(
-            client_id=client_id,
-            client_secret=client_secret,
-            callback_url=callback_url,
+        from twitter_api.api.types.oauth1.oauth1_authorization import (
+            OAuth1Authorization,
         )
 
-        return TwitterOAuth2AccessTokenClient(
-            authorization_response_url=authorization_response_url,
-            state=state,
-            code_verifier=code_verifier,
-            session=session,
+        return OAuth1Authorization(
+            authorization_url="https://authorization.url.com",
+            session=self,
         )
 
-    @classmethod
-    def from_authorization_response_url_env(
-        cls,
-        *,
-        client_id_env: Env[ClientId] = "CLIENT_ID",
-        client_secret_env: Env[ClientSecret] = "CLIENT_SECRET",
-        callback_url_env: Env[CallbackUrl] = "CALLBACK_URL",
+    def fetch_token(
+        self,
         authorization_response_url: CallbackUrl,
-        state: str,
-        code_verifier: str,
-        callback_url: Optional[CallbackUrl] = None,
     ):
-        return cls.from_authorization_response_url(
-            client_id=cls._get_env(client_id_env),
-            client_secret=cls._get_env(client_secret_env),
-            callback_url=(
-                cls._get_env(callback_url_env) if callback_url is None else callback_url
-            ),
-            authorization_response_url=authorization_response_url,
-            state=state,
-            code_verifier=code_verifier,
+        from twitter_api.api.types.oauth1.oauth1_access_token import OAuth1AccessToken
+
+        return OAuth1AccessToken(
+            oauth_token="oauth_token",
+            oauth_token_secret="oauth_token_secret",
+            user_id="user_id",
+            screen_name="screen_name",
+            _session=self,
         )
 
-    @classmethod
-    def _get_env(cls, key: Env[str]) -> str:
-        """環境変数を取り出す。"""
-        return os.environ[key]
+    def generate_client(self, access_token: AccessToken, access_secret: AccessSecret):
+        return self._client_generator(access_token, access_secret)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `twitter_api_py-0.1.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py` & `twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from dataclasses import dataclass
+from typing import Generic
 
 from twitter_api.client.oauth_session.resources.oauth2_authorize import (
     OAuth2AuthorizeSessionResources,
     Oauth2AuthorizeUrl,
 )
 from twitter_api.client.oauth_session.twitter_oauth2_session import TwitterOAuth2Session
 from twitter_api.types.chainable import Chainable
+from twitter_api.types.generic_client import TwitterApiGenericClient
 
 
 @dataclass
-class TwitterOAuth2AuthorizeClient(Chainable):
-    def __init__(self, session: TwitterOAuth2Session) -> None:
+class TwitterOAuth2AuthorizeClient(Chainable, Generic[TwitterApiGenericClient]):
+    def __init__(self, session: TwitterOAuth2Session[TwitterApiGenericClient]) -> None:
         self._session = session
 
-    def resource(self, url: Oauth2AuthorizeUrl) -> OAuth2AuthorizeSessionResources:
+    def request(
+        self, url: Oauth2AuthorizeUrl
+    ) -> OAuth2AuthorizeSessionResources[TwitterApiGenericClient]:
         return OAuth2AuthorizeSessionResources(
             self._session,
         )
```

### Comparing `twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py` & `twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,36 @@
-from twitter_api.api.types.oauth1.oauth1_access_token import OAuth1AccessToken
-from twitter_api.client.oauth_session.resources.session_resources import (
-    OAuth1SessionResources,
+from typing import Generic, Union
+
+from twitter_api.client.oauth_session.resources.oauth1_authenticate import (
+    OAuth1AuthenticateSessionResources,
+    OauthAuth1enticateUrl,
+)
+from twitter_api.client.oauth_session.resources.oauth1_authorize import (
+    OAuth1AuthorizeSessionResources,
+    Oauth1AuthorizeUrl,
 )
 from twitter_api.client.oauth_session.twitter_oauth1_session import TwitterOAuth1Session
-from twitter_api.types.oauth import CallbackUrl
-
-
-class PostOauth1AccessTokenResources(OAuth1SessionResources):
-    def __init__(
-        self,
-        authorization_response_url: CallbackUrl,
-        session: TwitterOAuth1Session,
-    ) -> None:
-        self._authorization_response_url = authorization_response_url
-        super().__init__(session)
+from twitter_api.error import NeverError
+from twitter_api.types.chainable import Chainable
+from twitter_api.types.generic_client import TwitterApiGenericClient
 
-    def post(
-        self,
-    ) -> OAuth1AccessToken:
-        """
-        OAuth 1.0a の最後のステップ。
-        ユーザーアクセストークンのセットを生成する。
 
-        refer: https://developer.twitter.com/en/docs/authentication/api-reference/access_token
-        """
+class TwitterOAuth1AuthorizeClient(Chainable, Generic[TwitterApiGenericClient]):
+    def __init__(self, session: TwitterOAuth1Session[TwitterApiGenericClient]) -> None:
+        self._session = session
 
-        return self._session.fetch_token(self._authorization_response_url)
+    def request(
+        self, url: OauthAuth1enticateUrl | Oauth1AuthorizeUrl
+    ) -> Union[
+        OAuth1AuthenticateSessionResources[TwitterApiGenericClient],
+        OAuth1AuthorizeSessionResources[TwitterApiGenericClient],
+    ]:
+        if url == "https://api.twitter.com/oauth/authenticate":
+            return OAuth1AuthenticateSessionResources(
+                self._session,
+            )
+        elif url == "https://api.twitter.com/oauth/authorize":
+            return OAuth1AuthorizeSessionResources(
+                self._session,
+            )
+        else:
+            raise NeverError(url)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py` & `twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from twitter_api.client.oauth_session.resources.session_resources import (
     OAuth1SessionResources,
 )
+from twitter_api.types.generic_client import TwitterApiGenericClient
 
 
 class GenerateAuthorizationUrlOAuth1AuthenticateSessionResources(
-    OAuth1SessionResources
+    OAuth1SessionResources[TwitterApiGenericClient]
 ):
     def generate_authorization_url(self):
         """
         OAuth 1.0a の 2 番目のステップ。
         ユーザーアクセストークンのセットを生成するために、
         Twitter 認証用のページへのアクセス用 URL を生成する。
```

### Comparing `twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py` & `twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from twitter_api.client.oauth_session.resources.session_resources import (
     OAuth1SessionResources,
 )
+from twitter_api.types.generic_client import TwitterApiGenericClient
 
 
-class GenerateAuthorizationUrlOAuth1AuthorizeSessionResources(OAuth1SessionResources):
+class GenerateAuthorizationUrlOAuth1AuthorizeSessionResources(
+    OAuth1SessionResources[TwitterApiGenericClient]
+):
     def generate_authorization_url(self):
         """
         OAuth 1.0a の 2 番目のステップ。
         ユーザーアクセストークンのセットを生成するために使用する。
 
         refer: https://developer.twitter.com/en/docs/authentication/api-reference/authorize
         """
```

### Comparing `twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py` & `twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from twitter_api.client.oauth_session.resources.session_resources import (
     OAuth2SessionResources,
 )
+from twitter_api.types.generic_client import TwitterApiGenericClient
 
 
-class GenerateAuthorizationUrlOAuth2AuthorizeSessionResources(OAuth2SessionResources):
+class GenerateAuthorizationUrlOAuth2AuthorizeSessionResources(
+    OAuth2SessionResources[TwitterApiGenericClient],
+):
     def generate_authorization_url(self):
         """
         OAuth 2.0 のユーザ認証（PKCE）の最初のステップ。
 
         ユーザーアクセストークンのセットを生成するために、
         Twitter 認証用のページへのアクセス用 URL を生成する。
 
         refer: https://developer.twitter.com/en/docs/authentication/oauth-2-0/authorization-code
         """
+
         return self._session.generate_authorization_url()
```

### Comparing `twitter_api_py-0.1.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py` & `twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,37 @@
+from typing import Generic
+
 from twitter_api.api.types.oauth2.oauth2_access_token import OAuth2AccessToken
 from twitter_api.client.oauth_session.resources.session_resources import (
     OAuth2SessionResources,
 )
 from twitter_api.client.oauth_session.twitter_oauth2_session import TwitterOAuth2Session
 from twitter_api.types.endpoint import Endpoint
-from twitter_api.types.http import Url
+from twitter_api.types.generic_client import TwitterApiGenericClient
 from twitter_api.types.oauth import CallbackUrl
 
 ENDPOINT = Endpoint("POST", "https://api.twitter.com/2/oauth2/token")
 
 
-class PostV2OAuth2TokenRerources(OAuth2SessionResources):
+class PostV2OAuth2TokenRerources(
+    OAuth2SessionResources, Generic[TwitterApiGenericClient]
+):
     def __init__(
         self,
         authorization_response_url: CallbackUrl,
         state: str,
         code_verifier: str,
-        session: TwitterOAuth2Session,
+        session: TwitterOAuth2Session[TwitterApiGenericClient],
     ) -> None:
         self._authorization_response_url = authorization_response_url
         self._state = state
         self._code_verifier = code_verifier
         super().__init__(session)
 
-    def post(self) -> OAuth2AccessToken:
+    def post(self) -> OAuth2AccessToken[TwitterApiGenericClient]:
         """
         OAuth2.0 のユーザ認証（PKCE）の最後のステップ。認証のトークンを発行する。
 
         API 専用のページはドキュメントに存在しない。
 
         refer: https://developer.twitter.com/en/docs/authentication/oauth-2-0/authorization-code
         """
```

### Comparing `twitter_api_py-0.1.0/twitter_api/client/oauth_session/twitter_oauth1_async_mock_session.py` & `twitter_api_py-0.2.0/twitter_api/api/types/oauth2/oauth2_access_token.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,24 @@
-from twitter_api.client.oauth_session.twitter_oauth1_mock_session import (
-    TwitterOAuth1MockSession,
-)
-from twitter_api.types.oauth import AccessSecret, AccessToken
+from typing import Generic
 
+from typing_extensions import Literal
 
-class TwitterOAuth1AsyncMockSession(TwitterOAuth1MockSession):
-    def generate_client(self, access_token: AccessToken, access_secret: AccessSecret):
-        from twitter_api.client.twitter_api_async_mock_client import (
-            TwitterApiAsyncMockClient,
-        )
+from twitter_api.api.types.v2_scope import Scope
+from twitter_api.client.oauth_session.twitter_oauth2_session import TwitterOAuth2Session
+from twitter_api.types.chainable import Chainable
+from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.generic_client import TwitterApiGenericClient
+from twitter_api.types.oauth import AccessToken
 
-        return TwitterApiAsyncMockClient.from_oauth1_app(
-            api_key="api_key",
-            api_secret="api_secret",
-            access_token=access_token,
-            access_secret=access_secret,
-        )
+
+class OAuth2AccessToken(
+    Chainable, ExtraPermissiveModel, Generic[TwitterApiGenericClient]
+):
+    token_type: Literal["bearer"]
+    expires_in: int
+    expires_at: int
+    access_token: AccessToken
+    scope: list[Scope]
+    _session: TwitterOAuth2Session[TwitterApiGenericClient]
+
+    def generate_client(self) -> TwitterApiGenericClient:
+        return self._session.generate_client(self.access_token)
```

### Comparing `twitter_api_py-0.1.0/twitter_api/client/oauth_session/twitter_oauth1_session.py` & `twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth1_session.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 from abc import ABCMeta, abstractmethod
+from typing import Generic
 
+from twitter_api.types.generic_client import TwitterApiGenericClient
 from twitter_api.types.http import Url
 from twitter_api.types.oauth import AccessSecret, AccessToken, CallbackUrl
 
 
-class TwitterOAuth1Session(metaclass=ABCMeta):
+class TwitterOAuth1Session(Generic[TwitterApiGenericClient], metaclass=ABCMeta):
     @abstractmethod
     def request_token(self):
-        # NOTE: 本来実装は不要だが、モジュールの循環読み込みを防ぐため、
-        #       偽のデータを作っている。
         from twitter_api.client.oauth_flow.twitter_oauth1_authorization_client import (
             TwitterOAuth1AuthorizeClient,
         )
 
-        return TwitterOAuth1AuthorizeClient(**{})
+        _: TwitterOAuth1AuthorizeClient[TwitterApiGenericClient] = ...  # type: ignore
+
+        return _
 
     @abstractmethod
     def generate_authorization_url(
         self,
         url: Url,
     ):
-        # NOTE: 本来実装は不要だが、モジュールの循環読み込みを防ぐため、
-        #       偽のデータを作っている。
         from twitter_api.api.types.oauth1.oauth1_authorization import (
             OAuth1Authorization,
         )
 
-        return OAuth1Authorization(**{})
+        _: OAuth1Authorization[TwitterApiGenericClient] = ...  # type: ignore
+
+        return _
 
     @abstractmethod
     def fetch_token(
         self,
         authorization_response_url: CallbackUrl,
     ):
         # NOTE: 本来実装は不要だが、モジュールの循環読み込みを防ぐため、
         #       偽のデータを作っている。
         from twitter_api.api.types.oauth1.oauth1_access_token import OAuth1AccessToken
 
-        return OAuth1AccessToken(**{})
+        _: OAuth1AccessToken[TwitterApiGenericClient] = ...  # type: ignore
 
-    @abstractmethod
-    def generate_client(self, access_token: AccessToken, access_secret: AccessSecret):
-        # NOTE: 本来実装は不要だが、モジュールの循環読み込みを防ぐため、
-        #       偽のデータを作っている。
-        from twitter_api.client.twitter_api_client import TwitterApiClient
+        return _
 
-        return TwitterApiClient.from_oauth1_app(**{})
+    @abstractmethod
+    def generate_client(
+        self, access_token: AccessToken, access_secret: AccessSecret
+    ) -> TwitterApiGenericClient:
+        ...
```

### Comparing `twitter_api_py-0.1.0/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py` & `twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 from datetime import datetime
+from typing import Callable
 
 from twitter_api.api.types.oauth2.oauth2_access_token import OAuth2AccessToken
 from twitter_api.api.types.v2_scope import Scope
 from twitter_api.client.oauth_session.twitter_oauth2_session import TwitterOAuth2Session
-from twitter_api.types.oauth import CallbackUrl
+from twitter_api.types.generic_client import TwitterApiGenericMockClient
+from twitter_api.types.oauth import AccessToken, CallbackUrl
 
 
-class TwitterOAuth2MockSession(TwitterOAuth2Session):
-    def __init__(self, *, scope: list[Scope]) -> None:
+class TwitterOAuth2MockSession(TwitterOAuth2Session[TwitterApiGenericMockClient]):
+    def __init__(
+        self,
+        client_generator: Callable[[AccessToken], TwitterApiGenericMockClient],
+        *,
+        scope: list[Scope],
+    ) -> None:
+        self._client_generator = client_generator
         self._scope = scope
 
     def generate_authorization_url(self):
         from twitter_api.api.types.oauth2.oauth2_authorization import (
             OAuth2Authorization,
         )
 
@@ -34,11 +42,9 @@
             expires_in=expires_in,
             expires_at=int(datetime.now().timestamp()) + expires_in,
             access_token="access_token",
             scope=self._scope,
             _session=self,
         )
 
-    def generate_client(self, access_token: str):
-        from twitter_api.client.twitter_api_mock_client import TwitterApiMockClient
-
-        return TwitterApiMockClient.from_oauth2_bearer_token(bearer_token=access_token)
+    def generate_client(self, access_token: AccessToken):
+        return self._client_generator(access_token)
```

### Comparing `twitter_api_py-0.1.0/twitter_api/client/request/request_async_client.py` & `twitter_api_py-0.2.0/twitter_api/client/request/request_async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,46 +14,49 @@
 
 class RequestAsyncClient(RequestClient):
     @abstractmethod
     async def get(
         self,
         *,
         endpoint: Endpoint,
-        response_type: Type[ResponseModelBody],
+        response_body_type: Type[ResponseModelBody],
         url: Optional[Url] = None,
         auth: bool = True,
         query: Optional[QuryParameters] = None,
     ) -> ResponseModelBody:
         ...
 
     @abstractmethod
     async def post(
         self,
         *,
         endpoint: Endpoint,
-        response_type: Type[ResponseModelBody],
+        response_body_type: Type[ResponseModelBody],
         url: Optional[Url] = None,
         auth: bool = True,
         headers: Optional[Headers] = None,
         query: Optional[QuryParameters] = None,
         body: Optional[RequestJsonBody] = None,
     ) -> ResponseModelBody:
         ...
 
     @abstractmethod
     async def delete(
         self,
         *,
         endpoint: Endpoint,
-        response_type: Type[ResponseModelBody],
+        response_body_type: Type[ResponseModelBody],
         url: Optional[Url] = None,
         auth: bool = True,
         headers: Optional[Headers] = None,
         query: Optional[QuryParameters] = None,
     ) -> ResponseModelBody:
         ...
 
+    async def aclose(self) -> None:
+        pass
+
     async def __aenter__(self) -> Self:
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback) -> None:
         pass
```

### Comparing `twitter_api_py-0.1.0/twitter_api/client/request/request_async_real_client.py` & `twitter_api_py-0.2.0/twitter_api/client/request/request_async_real_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Optional, Self, Type
+from typing import Mapping, Optional, Self, Type
 
-import httpx
 from authlib.integrations.httpx_client.oauth1_client import OAuth1Auth
 from authlib.integrations.httpx_client.oauth2_client import OAuth2Auth
 
 from twitter_api.client.request.request_async_client import RequestAsyncClient
 from twitter_api.client.request.request_real_client import (
     _parse_response,
     _remove_none_field,
 )
 from twitter_api.rate_limit.manager.no_operation_rate_limit_manager import (
     NoOperationRateLimitManager,
 )
 from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
-from twitter_api.rate_limit.rate_limit_target import RateLimitTarget
+from twitter_api.rate_limit.types.rate_limit_target import RateLimitTarget
+from twitter_api.types import httpx
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.http import Url
 from twitter_api.types.oauth import OAuthVersion
 
 from .request_client import Headers, QuryParameters, RequestJsonBody, ResponseModelBody
 
 OAuth = OAuth2Auth | OAuth1Auth
@@ -26,26 +26,39 @@
 class RequestAsyncRealClient(RequestAsyncClient):
     def __init__(
         self,
         *,
         auth: Optional[OAuth],
         oauth_version: OAuthVersion,
         rate_limit_target: RateLimitTarget,
-        rate_limit_manager: Optional[RateLimitManager] = None,
+        rate_limit_manager: RateLimitManager,
+        event_hooks: Optional[Mapping[str, list[httpx.EventHook]]],
+        limits: httpx.Limits,
+        mounts: Optional[Mapping[str, httpx.AsyncBaseTransport]],
+        proxies: Optional[httpx.ProxiesTypes],
+        timeout: httpx.TimeoutTypes,
+        transport: Optional[httpx.AsyncBaseTransport],
+        verify: httpx.VerifyTypes,
         session: Optional[httpx.AsyncClient] = None,
-        timeout_sec: Optional[float] = None,
     ) -> None:
         if session is None:
-            session = httpx.AsyncClient()
+            session = httpx.AsyncClient(
+                event_hooks=event_hooks,
+                limits=limits,
+                mounts=mounts,
+                proxies=proxies,
+                timeout=timeout,
+                transport=transport,
+                verify=verify,
+            )
 
         self._oauth_version: OAuthVersion = oauth_version
         self._rate_limit_target: RateLimitTarget = rate_limit_target
         self._auth = auth
         self._session = session
-        self.timeout_sec = timeout_sec
 
         if rate_limit_manager is None:
             rate_limit_manager = NoOperationRateLimitManager()
 
         self._rate_limit_manager = rate_limit_manager
 
     @property
@@ -60,46 +73,45 @@
     def rate_limit_manager(self) -> RateLimitManager:
         return self._rate_limit_manager
 
     async def get(
         self,
         *,
         endpoint: Endpoint,
-        response_type: Type[ResponseModelBody],
+        response_body_type: Type[ResponseModelBody],
         url: Optional[Url] = None,
         auth: bool = True,
         headers: Optional[Headers] = None,
         query: Optional[QuryParameters] = None,
         body: Optional[RequestJsonBody] = None,
     ) -> ResponseModelBody:
         url = endpoint.url if url is None else url
 
         response = await self._session.request(
             url=url,
             auth=self._auth if auth else None,
             method=endpoint.method,
             params=_remove_none_field(query),
-            timeout=self.timeout_sec,
         )
 
         return _parse_response(
             endpoint,
             response,
-            response_type,
+            response_body_type,
             url,
             headers,
             query,
             body,
         )
 
     async def post(
         self,
         *,
         endpoint: Endpoint,
-        response_type: Type[ResponseModelBody],
+        response_body_type: Type[ResponseModelBody],
         url: Optional[Url] = None,
         auth: bool = True,
         headers: Optional[Headers] = None,
         query: Optional[QuryParameters] = None,
         body: Optional[RequestJsonBody] = None,
     ) -> ResponseModelBody:
         url = endpoint.url if url is None else url
@@ -107,62 +119,57 @@
         response = await self._session.request(
             url=url,
             auth=self._auth if auth else None,
             method=endpoint.method,
             headers=headers,
             params=_remove_none_field(query),
             json=_remove_none_field(body),
-            timeout=self.timeout_sec,
         )
 
-        if response_type is str:
-            return response.content.decode("utf-8")  # type: ignore
-
         return _parse_response(
             endpoint,
             response,
-            response_type,
+            response_body_type,
             url,
             headers,
             query,
             body,
         )
 
     async def delete(
         self,
         *,
         endpoint: Endpoint,
-        response_type: Type[ResponseModelBody],
+        response_body_type: Type[ResponseModelBody],
         url: Optional[Url] = None,
         auth: bool = True,
         headers: Optional[Headers] = None,
         query: Optional[QuryParameters] = None,
     ) -> ResponseModelBody:
         url = endpoint.url if url is None else url
 
         response = await self._session.request(
             url=url,
             auth=self._auth if auth else None,
             method=endpoint.method,
             headers=headers,
             params=_remove_none_field(query),
-            timeout=self.timeout_sec,
         )
 
-        if response_type is str:
-            return response.content.decode("utf-8")  # type: ignore
-
         return _parse_response(
             endpoint,
             response,
-            response_type,
+            response_body_type,
             url,
             headers,
             query,
         )
 
+    async def aclose(self) -> None:
+        await self._session.aclose()
+
     async def __aenter__(self) -> Self:
         await self._session.__aenter__()
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback) -> None:
         await self._session.__aexit__(exc_type, exc_value, traceback)
```

### Comparing `twitter_api_py-0.1.0/twitter_api/client/request/request_mock_client.py` & `twitter_api_py-0.2.0/twitter_api/client/request/request_mock_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     MockResponseNotFound,
     TwitterApiError,
 )
 from twitter_api.rate_limit.manager.no_operation_rate_limit_manager import (
     NoOperationRateLimitManager,
 )
 from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
-from twitter_api.rate_limit.rate_limit_target import RateLimitTarget
+from twitter_api.rate_limit.types.rate_limit_target import RateLimitTarget
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.http import Url
 from twitter_api.types.oauth import OAuthVersion
 
 from .request_client import (
     Headers,
     QuryParameters,
@@ -25,15 +25,15 @@
 
 class RequestMockClient(RequestClient, Generic[ResponseModelBody]):
     def __init__(
         self,
         *,
         oauth_version: OAuthVersion,
         rate_limit_target: RateLimitTarget,
-        rate_limit_manager: Optional[RateLimitManager] = None,
+        rate_limit_manager: RateLimitManager,
     ):
         self._store: list[tuple[Endpoint, ResponseModelBody | TwitterApiError]] = []
         self._oauth_version: OAuthVersion = oauth_version
         self._rate_limit_target: RateLimitTarget = rate_limit_target
 
         if rate_limit_manager is None:
             rate_limit_manager = NoOperationRateLimitManager()
@@ -71,38 +71,38 @@
 
         return response_body
 
     def get(
         self,
         *,
         endpoint: Endpoint,
-        response_type: Type[ResponseModelBody],
+        response_body_type: Type[ResponseModelBody],
         url: Optional[Url] = None,
         auth: bool = True,
         query: Optional[QuryParameters] = None,
     ) -> ResponseModelBody:
         return self._extract_response_body(endpoint)
 
     def post(
         self,
         *,
         endpoint: Endpoint,
-        response_type: Type[ResponseModelBody],
+        response_body_type: Type[ResponseModelBody],
         url: Optional[Url] = None,
         auth: bool = True,
         headers: Optional[Headers] = None,
         query: Optional[QuryParameters] = None,
         body: Optional[RequestJsonBody] = None,
     ) -> ResponseModelBody:
         return self._extract_response_body(endpoint)
 
     def delete(
         self,
         *,
         endpoint: Endpoint,
-        response_type: Type[ResponseModelBody],
+        response_body_type: Type[ResponseModelBody],
         url: Optional[Url] = None,
         auth: bool = True,
         headers: Optional[Headers] = None,
         query: Optional[QuryParameters] = None,
     ) -> ResponseModelBody:
         return self._extract_response_body(endpoint)
```

### Comparing `twitter_api_py-0.1.0/twitter_api/client/request/request_real_client.py` & `twitter_api_py-0.2.0/twitter_api/client/request/request_real_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from typing import Optional, Type
+from typing import Mapping, Optional, Self, Type
 
-import httpx
 import pydantic
 from authlib.integrations.httpx_client.oauth1_client import OAuth1Auth
 from authlib.integrations.httpx_client.oauth2_client import OAuth2Auth
 
 from twitter_api.error import (
     TwitterApiOAuthTokenV1NotFound,
     TwitterApiResponseError,
@@ -12,15 +11,16 @@
     TwitterApiResponseModelBodyDecodeError,
     TwitterApiResponseValidationError,
 )
 from twitter_api.rate_limit.manager.no_operation_rate_limit_manager import (
     NoOperationRateLimitManager,
 )
 from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
-from twitter_api.rate_limit.rate_limit_target import RateLimitTarget
+from twitter_api.rate_limit.types.rate_limit_target import RateLimitTarget
+from twitter_api.types import httpx
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.http import Url
 from twitter_api.types.oauth import OAuthVersion
 
 from .request_client import (
     Headers,
     QuryParameters,
@@ -35,26 +35,39 @@
 class RequestRealClient(RequestClient):
     def __init__(
         self,
         *,
         auth: Optional[OAuth],
         oauth_version: OAuthVersion,
         rate_limit_target: RateLimitTarget,
-        rate_limit_manager: Optional[RateLimitManager] = None,
+        rate_limit_manager: RateLimitManager,
+        event_hooks: Optional[Mapping[str, list[httpx.EventHook]]],
+        limits: httpx.Limits,
+        mounts: Optional[Mapping[str, httpx.BaseTransport]],
+        proxies: Optional[httpx.ProxiesTypes],
+        timeout: httpx.TimeoutTypes,
+        transport: Optional[httpx.BaseTransport],
+        verify: httpx.VerifyTypes,
         session: Optional[httpx.Client] = None,
-        timeout_sec: Optional[float] = None,
     ) -> None:
         if session is None:
-            session = httpx.Client()
+            session = httpx.Client(
+                event_hooks=event_hooks,
+                limits=limits,
+                mounts=mounts,
+                proxies=proxies,
+                timeout=timeout,
+                transport=transport,
+                verify=verify,
+            )
 
         self._oauth_version: OAuthVersion = oauth_version
         self._rate_limit_target: RateLimitTarget = rate_limit_target
         self._auth = auth
         self._session = session
-        self.timeout_sec = timeout_sec
 
         if rate_limit_manager is None:
             rate_limit_manager = NoOperationRateLimitManager()
 
         self._rate_limit_manager = rate_limit_manager
 
     @property
@@ -69,46 +82,45 @@
     def rate_limit_manager(self) -> RateLimitManager:
         return self._rate_limit_manager
 
     def get(
         self,
         *,
         endpoint: Endpoint,
-        response_type: Type[ResponseModelBody],
+        response_body_type: Type[ResponseModelBody],
         url: Optional[Url] = None,
         auth: bool = True,
         headers: Optional[Headers] = None,
         query: Optional[QuryParameters] = None,
         body: Optional[RequestJsonBody] = None,
     ) -> ResponseModelBody:
         url = endpoint.url if url is None else url
 
         response = self._session.request(
             url=url,
             auth=self._auth if auth else None,
             method=endpoint.method,
             params=_remove_none_field(query),
-            timeout=self.timeout_sec,
         )
 
         return _parse_response(
             endpoint,
             response,
-            response_type,
+            response_body_type,
             url,
             headers,
             query,
             body,
         )
 
     def post(
         self,
         *,
         endpoint: Endpoint,
-        response_type: Type[ResponseModelBody],
+        response_body_type: Type[ResponseModelBody],
         url: Optional[Url] = None,
         auth: bool = True,
         headers: Optional[Headers] = None,
         query: Optional[QuryParameters] = None,
         body: Optional[RequestJsonBody] = None,
     ) -> ResponseModelBody:
         url = endpoint.url if url is None else url
@@ -116,68 +128,71 @@
         response = self._session.request(
             url=url,
             auth=self._auth if auth else None,
             method=endpoint.method,
             headers=headers,
             params=_remove_none_field(query),
             json=_remove_none_field(body),
-            timeout=self.timeout_sec,
         )
 
-        if response_type is str:
-            return response.content.decode("utf-8")  # type: ignore
-
         return _parse_response(
             endpoint,
             response,
-            response_type,
+            response_body_type,
             url,
             headers,
             query,
             body,
         )
 
     def delete(
         self,
         *,
         endpoint: Endpoint,
-        response_type: Type[ResponseModelBody],
+        response_body_type: Type[ResponseModelBody],
         url: Optional[Url] = None,
         auth: bool = True,
         headers: Optional[Headers] = None,
         query: Optional[QuryParameters] = None,
     ) -> ResponseModelBody:
         url = endpoint.url if url is None else url
 
         response = self._session.request(
             url=url,
             auth=self._auth if auth else None,
             method=endpoint.method,
             headers=headers,
             params=_remove_none_field(query),
-            timeout=self.timeout_sec,
         )
 
-        if response_type is str:
-            return response.content.decode("utf-8")  # type: ignore
-
         return _parse_response(
             endpoint,
             response,
-            response_type,
+            response_body_type,
             url,
             headers,
             query,
         )
 
+    def close(self) -> None:
+        self._session.close()
+
+    def __enter__(self) -> Self:
+        self._session = self._session.__enter__()
+
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback) -> None:
+        self._session.__exit__(exc_type, exc_value, traceback)
+
 
 def _parse_response(
     endpoint: Endpoint,
     response: httpx.Response,
-    response_type: Type[ResponseModelBody],
+    response_body_type: Type[ResponseModelBody],
     url: Url,
     headers: Optional[Headers] = None,
     query: Optional[QuryParameters] = None,
     body: Optional[RequestJsonBody] = None,
 ) -> ResponseModelBody:
     if response.content == b"":
         data: dict = {}
@@ -223,15 +238,15 @@
     if "reason" in data:
         raise TwitterApiOAuthTokenV1NotFound(
             endpoint,
             data,
         )
 
     try:
-        return response_type(**data)
+        return response_body_type(**data)
     except pydantic.ValidationError as error:
         raise TwitterApiResponseValidationError(endpoint, data, error)
 
 
 def _remove_none_field(data: Optional[dict]) -> Optional[dict]:
     if data is None:
         return None
```

### Comparing `twitter_api_py-0.1.0/twitter_api/error.py` & `twitter_api_py-0.2.0/twitter_api/error.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 import json
+from abc import abstractmethod
 from collections import OrderedDict
 from enum import Enum
 from textwrap import dedent
 from typing import Any, Never, Optional
 
 import pydantic
 
-from twitter_api.rate_limit.rate_limit_info import RateLimitInfo
+from twitter_api.rate_limit.types.rate_limit_info import RateLimitInfo
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 
 from .types.endpoint import Endpoint
 from .types.http import Headers, QuryParameters, RequestJsonBody, ResponseJsonBody
 from .types.oauth import OAuthVersion
-from .utils.json import exclude_none
+from .utils._functional import exclude_none
 
 
-class ErrorMessage(ExtraPermissiveModel):
+class TwitterApiExceptionInfo(ExtraPermissiveModel):
     type: str
     message: str
     erros: Optional[list[str]] = None
 
-    def to_message(self) -> str:
-        return self.json()
-
 
 class TwitterApiException(Exception):
     ...
 
+    @property
+    @abstractmethod
+    def message(self) -> str:
+        ...
+
+    @property
+    def info(self) -> TwitterApiExceptionInfo:
+        return TwitterApiExceptionInfo(
+            type=self.__class__.__name__,
+            message=self.message,
+        )
+
+    def __str__(self) -> str:
+        return self.message
+
 
 class TwitterApiError(TwitterApiException):
     ...
 
 
 class TwitterApiErrorCode(Enum):
     """
@@ -52,104 +65,74 @@
     TooManyRequests = 429
     InternalServerError = 500
     BadGateway = 502
     ServiceUnavailable = 503
     GatewayTimeout = 504
 
 
-def code2message(error_code: int):
-    match error_code:
-        case TwitterApiErrorCode.OK.value:
-            return "API が成功しています。"
-        case TwitterApiErrorCode.NotModified.value:
-            return "返却する新しいデータがありません。"
-        case TwitterApiErrorCode.BadRequest.value:
-            return "リクエストの形式が間違っています。"
-        case TwitterApiErrorCode.Unauthorized.value:
-            return "このリクエストは証認されていません。"
-        case TwitterApiErrorCode.Forbidden.value:
-            return "このリクエストは許可されていません。"
-        case TwitterApiErrorCode.NotFound.value:
-            return "データが見つかりません。"
-        case TwitterApiErrorCode.NotAcceptable.value:
-            return "アクセスできません。"
-        case TwitterApiErrorCode.ConnectionException.value:
-            return "接続に失敗しました。"
-        case TwitterApiErrorCode.Gone.value:
-            return "このリソースは利用できなくなりました。"
-        case TwitterApiErrorCode.UnprocessableEntity.value:
-            return "処理できないエンティティです。"
-        case TwitterApiErrorCode.TooManyRequests.value:
-            return "レートリミットか Tweet Cap が制限を超えました。"
-        case TwitterApiErrorCode.InternalServerError.value:
-            return "Twitter API の内部でエラーが発生しました。"
-        case TwitterApiErrorCode.BadGateway.value:
-            return "Twitter API がダウンしているか、アップグレード中です。"
-        case TwitterApiErrorCode.ServiceUnavailable.value:
-            return "リクエスト数が多く処理できません。後でもう一度お試しください。"
-        case TwitterApiErrorCode.GatewayTimeout.value:
-            return "Twitter API が内部的にダウンしています。後でもう一度お試しください。"
-        case _:
-            return "Twitter API の応答が 200 ではありません。"
-
-
 class NeverError(TwitterApiError):
     def __init__(self, never: Never):
         self._never = never
 
-    def __str__(self) -> str:
-        return ErrorMessage(
-            type=self.__class__.__name__,
-            message=f'到達できない入力 "{self._never}" が与えられました。',
-        ).to_message()
+    @property
+    def message(self) -> str:
+        return f'到達できないはずの入力 "{self._never}" が与えられました。'
 
 
 class MockResponseNotFound(TwitterApiError):
-    def __str__(self) -> str:
-        return ErrorMessage(
-            type=self.__class__.__name__,
-            message=dedent(
-                """
-                モックとして出力したいデータが入力されていません。
-                `client.inject_*(response)` で定義されているメソッドを用い、
-                レスポンスデータを定義した後で、API を呼んでください。
-                """
-            ),
-        ).to_message()
+    @property
+    def message(self) -> str:
+        return dedent(
+            """
+            モックとして出力したいデータが入力されていません。
+            `client.inject_*(response)` で定義されているメソッドを用い、
+            レスポンスデータを定義した後で、API を呼んでください。
+            """
+        )
 
 
 class MockInjectionResponseWrong(TwitterApiError):
     def __init__(self, endpoint: Endpoint, expected_endpoint: Endpoint):
         self._endpoint = endpoint
         self._expected_endpoint = expected_endpoint
 
-    def __str__(self) -> str:
-        return ErrorMessage(
+    @property
+    def message(self) -> str:
+        return "出力したいレスポンスのエンドポイントが異なっています。"
+
+    @property
+    def info(self) -> TwitterApiExceptionInfo:
+        return TwitterApiExceptionInfo(
             type=self.__class__.__name__,
-            message=("出力したいレスポンスのエンドポイントが異なっています。"),
+            message=self.message,
             **dict(
                 expected_endpoint=self._expected_endpoint,
                 endpoint=self._endpoint,
             ),
-        ).to_message()
+        )
 
 
 class TwitterApiResponseModelBodyDecodeError(TwitterApiError):
     def __init__(self, endpoint: Endpoint, content: bytes, **extra):
         self._endpoint = endpoint
         self._content = content
         self._extra = extra
 
-    def __str__(self) -> str:
-        return ErrorMessage(
+    @property
+    def message(self) -> str:
+        return "Twitter API の応答のボディを JSON でパースできませんでした。"
+
+    @property
+    def info(self) -> TwitterApiExceptionInfo:
+        return TwitterApiExceptionInfo(
             type=self.__class__.__name__,
-            message="Twitter API の応答のボディを JSON でパースできませんでした。",
+            message=self.message,
             **dict(endpoint=self._endpoint, content=self._content),
             **exclude_none(self._extra),
-        ).to_message()
+        )
 
 
 class TwitterApiResponseFailed(TwitterApiError):
     def __init__(
         self,
         endpoint: Endpoint,
         url: str,
@@ -163,125 +146,172 @@
         self._url = url
         self._request_headers = request_headers
         self._query = query
         self._request_body = request_body
         self.status_code = response_status_code
         self._response_body = response_body
 
-    def __str__(self) -> str:
-        return ErrorMessage(
+    @property
+    def message(self) -> str:
+        match self.status_code:
+            case TwitterApiErrorCode.OK.value:
+                return "API が成功しています。"
+            case TwitterApiErrorCode.NotModified.value:
+                return "返却する新しいデータがありません。"
+            case TwitterApiErrorCode.BadRequest.value:
+                return "リクエストの形式が間違っています。"
+            case TwitterApiErrorCode.Unauthorized.value:
+                return "このリクエストは証認されていません。"
+            case TwitterApiErrorCode.Forbidden.value:
+                return "このリクエストは許可されていません。"
+            case TwitterApiErrorCode.NotFound.value:
+                return "データが見つかりません。"
+            case TwitterApiErrorCode.NotAcceptable.value:
+                return "アクセスできません。"
+            case TwitterApiErrorCode.ConnectionException.value:
+                return "接続に失敗しました。"
+            case TwitterApiErrorCode.Gone.value:
+                return "このリソースは利用できなくなりました。"
+            case TwitterApiErrorCode.UnprocessableEntity.value:
+                return "処理できないエンティティです。"
+            case TwitterApiErrorCode.TooManyRequests.value:
+                return "レートリミットか Tweet Cap が制限を超えました。"
+            case TwitterApiErrorCode.InternalServerError.value:
+                return "Twitter API の内部でエラーが発生しました。"
+            case TwitterApiErrorCode.BadGateway.value:
+                return "Twitter API がダウンしているか、アップグレード中です。"
+            case TwitterApiErrorCode.ServiceUnavailable.value:
+                return "リクエスト数が多く処理できません。後でもう一度お試しください。"
+            case TwitterApiErrorCode.GatewayTimeout.value:
+                return "Twitter API が内部的にダウンしています。後でもう一度お試しください。"
+            case _:
+                return "Twitter API の応答が 200 ではありません。"
+
+    @property
+    def info(self) -> TwitterApiExceptionInfo:
+        return TwitterApiExceptionInfo(
             type=self.__class__.__name__,
-            message=code2message(self.status_code),
+            message=self.message,
             **OrderedDict(
                 endpoint=self._endpoint,
                 url=self._url,
                 reqeust_headers=exclude_none(self._request_headers),
                 query=exclude_none(self._query),
                 request_body=exclude_none(self._request_body),
                 response_status_code=self.status_code,
                 response_body=(
                     exclude_none(self._response_body)
                     if not isinstance(self._response_body, bytes)
                     else self._response_body
                 ),
             ),
-        ).to_message()
+        )
 
 
 class OAuth2UserAccessTokenExpired(TwitterApiError):
-    def __str__(self) -> str:
-        return ErrorMessage(
-            type=self.__class__.__name__,
-            message="OAuth2.0 のユーザ認証の ACCESS_TOKEN が失効しました。再度発行してください。",
-        ).to_message()
+    @property
+    def message(self) -> str:
+        return "OAuth2.0 のユーザ認証の ACCESS_TOKEN が失効しました。再度発行してください。"
 
 
 class TwitterApiResponseError(TwitterApiError):
     def __init__(self, endpoint: Endpoint, data: Any, **extra):
         self._endpoint = endpoint
         self._data = data
         self._extra = extra
 
-    def __str__(self) -> str:
-        return ErrorMessage(
+    @property
+    def message(self) -> str:
+        return "Twitter API の応答でエラーが返りました。"
+
+    @property
+    def info(self) -> TwitterApiExceptionInfo:
+        return TwitterApiExceptionInfo(
             type=self.__class__.__name__,
-            message="Twitter API の応答でエラーが返りました。",
+            message=self.message,
             **dict(
                 endpoint=self._endpoint,
                 data=exclude_none(self._data),
             ),
             **exclude_none(self._extra),
-        ).to_message()
+        )
 
 
 class TwitterApiResponseValidationError(TwitterApiError):
     def __init__(
         self, endpoint: Endpoint, response_body: Any, error: pydantic.ValidationError
     ):
         self._endpoint = endpoint
         self._response_body = response_body
         self._error = error
 
-    def __str__(self) -> str:
+    @property
+    def message(self) -> str:
+        return "Twitter API の応答の型が想定とは一致していません。"
+
+    @property
+    def info(self) -> TwitterApiExceptionInfo:
         response_body = exclude_none(self._response_body)
 
         # 文字が長すぎる場合、切り取る。
         response_body_str = json.dumps(response_body, ensure_ascii=False)
         max_length = 1000
         if len(response_body_str) > max_length:
             response_body = response_body_str[: max_length - 3] + "..."
 
-        return ErrorMessage(
+        return TwitterApiExceptionInfo(
             type=self.__class__.__name__,
-            message="Twitter API の応答の型が想定とは一致していません。",
+            message=self.message,
             **dict(
                 endpoint=self._endpoint,
                 response_body=response_body,
                 error=self._error.errors(),
             ),
-        ).to_message()
+        )
 
 
 class TwitterApiOAuthTokenV1NotFound(TwitterApiError):
     def __init__(self, endpoint, data: Any, **extra):
         self._endpoint = endpoint
         self._data = data
         self._extra = extra
 
-    def __str__(self) -> str:
-        return ErrorMessage(
+    @property
+    def message(self) -> str:
+        return "OAuth V1 のトークンが見つかりませんでした。"
+
+    @property
+    def info(self) -> TwitterApiExceptionInfo:
+        return TwitterApiExceptionInfo(
             type=self.__class__.__name__,
-            message="OAuth V1 のトークンが見つかりませんでした。",
+            message=self.message,
             **dict(
                 endpoint=self._endpoint,
                 data=exclude_none(self._data),
             ),
             **exclude_none(self._extra),
-        ).to_message()
+        )
 
 
 class TwitterApiOAuthVersionWrong(TwitterApiError):
     def __init__(self, *, version: OAuthVersion, expected_version: OAuthVersion):
         self._version = version
         self._expected_version = expected_version
 
-    def __str__(self) -> str:
-        return ErrorMessage(
-            type=self.__class__.__name__,
-            message=(
-                f'OAuth のバージョンは "{self._version}" ではなく'
-                f' "{self._expected_version}" である必要があります。'
-            ),
-        ).to_message()
+    @property
+    def message(self) -> str:
+        return f'OAuth のバージョンは "{self._version}" ではなく "{self._expected_version}" である必要があります。'
 
 
 class RateLimitOverError(TwitterApiError):
     def __init__(self, rate_limit: RateLimitInfo) -> None:
         self._rate_limit = rate_limit
 
-    def __str__(self) -> str:
+    @property
+    def message(self) -> str:
         return f"レートリミットを超えています。{self._rate_limit}"
 
 
 class UnsupportedAuthenticationError(TwitterApiError):
-    def __str__(self) -> str:
+    @property
+    def message(self) -> str:
         return "この認証方法でのアクセスは許可されていません。"
```

### Comparing `twitter_api_py-0.1.0/twitter_api/rate_limit/manager/dict_rate_limit_manager.py` & `twitter_api_py-0.2.0/twitter_api/rate_limit/manager/dict_rate_limit_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from typing import Optional
 
 from twitter_api.rate_limit.manager.handlers.raise_rate_limit_handler import (
     RaiseRateLimitHandler,
 )
-from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
-from twitter_api.rate_limit.rate_limit_info import RateLimitInfo
+from twitter_api.rate_limit.types.rate_limit_info import RateLimitInfo
 
 
 @dataclass
 class RateLimitStatus:
     start_datetime: datetime
     request_datetimes: list[datetime]
```

### Comparing `twitter_api_py-0.1.0/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py` & `twitter_api_py-0.2.0/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.1.0/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py` & `twitter_api_py-0.2.0/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from contextlib import asynccontextmanager, contextmanager
 from typing import AsyncGenerator, Generator
 
 from twitter_api.error import RateLimitOverError
 from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
-from twitter_api.rate_limit.rate_limit_info import RateLimitInfo
+from twitter_api.rate_limit.types.rate_limit_info import RateLimitInfo
 
 
 class RaiseRateLimitHandler(RateLimitManager):
     """
     レートリミットオーバーが発生した場合、例外を投げるもっとも単純な handler。
     """
 
-    @asynccontextmanager
-    async def handle_rate_limit_async(
+    @contextmanager
+    def handle_rate_limit_sync(
         self, rate_limit_info: RateLimitInfo
-    ) -> AsyncGenerator[None, None]:
+    ) -> Generator[None, None, None]:
         """
-        非同期的な TwitterApiAsyncClient を用いている場合のレートリミットの処理方法。
+        同期的な TwitterApiClient を用いている場合のレートリミットの処理方法。
         """
 
         if self.check_limit_over(rate_limit_info) is not None:
             raise RateLimitOverError(rate_limit_info)
 
         yield
 
-    @contextmanager
-    def handle_rate_limit_sync(
+    @asynccontextmanager
+    async def handle_rate_limit_async(
         self, rate_limit_info: RateLimitInfo
-    ) -> Generator[None, None, None]:
+    ) -> AsyncGenerator[None, None]:
         """
-        同期的な TwitterApiClient を用いている場合のレートリミットの処理方法。
+        非同期的な TwitterApiAsyncClient を用いている場合のレートリミットの処理方法。
         """
 
         if self.check_limit_over(rate_limit_info) is not None:
             raise RateLimitOverError(rate_limit_info)
 
         yield
```

### Comparing `twitter_api_py-0.1.0/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py` & `twitter_api_py-0.2.0/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,73 +3,71 @@
 import time
 from abc import ABCMeta
 from contextlib import asynccontextmanager, contextmanager
 from logging import getLogger
 
 from twitter_api.error import TwitterApiErrorCode, TwitterApiResponseFailed
 from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
-from twitter_api.rate_limit.rate_limit_info import RateLimitInfo
+from twitter_api.rate_limit.types.rate_limit_info import RateLimitInfo
 from twitter_api.warning import RateLimitOverWarning, UnmanagedRateLimitOverWarning
 
 logger = getLogger(__file__)
 
 
 class SleepRateLimitHandler(RateLimitManager, metaclass=ABCMeta):
     """
-    レートリミットに遭遇した場合、スリープするマネージャ。
-
-    これ自体は抽象クラスなので、他の RateLimitManager と組み合わせる必要がある。
+    レートリミットに遭遇した場合、スリープする handler。
     """
 
     def random_sleep_seconds(self) -> float:
         """
         予期しないレートリミットに遭遇した場合にランダムに休む時間[秒]。
         """
 
         # デフォルトは 5 ~ 15 分。
         return random.randint(5 * 60, 15 * 60)
 
-    @asynccontextmanager
-    async def handle_rate_limit_async(self, rate_limit_info: RateLimitInfo):
+    @contextmanager
+    def handle_rate_limit_sync(self, rate_limit_info: RateLimitInfo):
         while True:
             # レートリミットを超えてしまっていたら、必要な待ち時間分だけ待つ。
             wait_time_seconds = self.check_limit_over(rate_limit_info)
             if wait_time_seconds is not None:
                 logger.warning(RateLimitOverWarning(rate_limit_info))
-                await asyncio.sleep(wait_time_seconds)
+                time.sleep(wait_time_seconds)
                 continue
 
             try:
                 yield
             except TwitterApiResponseFailed as error:
-                # レートリミットのエラーでないなら上流に投げる。
+                # レートリミット以外のエラーなら上流に投げる。
                 if error.status_code != TwitterApiErrorCode.TooManyRequests.value:
                     raise error
 
                 # 予期しないレートリミットに遭遇した場合、投機的な待機を行う
                 logger.warning(UnmanagedRateLimitOverWarning())
-                await asyncio.sleep(self.random_sleep_seconds())
+                time.sleep(self.random_sleep_seconds())
             else:
                 return
 
-    @contextmanager
-    def handle_rate_limit_sync(self, rate_limit_info: RateLimitInfo):
+    @asynccontextmanager
+    async def handle_rate_limit_async(self, rate_limit_info: RateLimitInfo):
         while True:
             # レートリミットを超えてしまっていたら、必要な待ち時間分だけ待つ。
             wait_time_seconds = self.check_limit_over(rate_limit_info)
             if wait_time_seconds is not None:
                 logger.warning(RateLimitOverWarning(rate_limit_info))
-                time.sleep(wait_time_seconds)
+                await asyncio.sleep(wait_time_seconds)
                 continue
 
             try:
                 yield
             except TwitterApiResponseFailed as error:
-                # レートリミット以外のエラーなら上流に投げる。
+                # レートリミットのエラーでないなら上流に投げる。
                 if error.status_code != TwitterApiErrorCode.TooManyRequests.value:
                     raise error
 
                 # 予期しないレートリミットに遭遇した場合、投機的な待機を行う
                 logger.warning(UnmanagedRateLimitOverWarning())
-                time.sleep(self.random_sleep_seconds())
+                await asyncio.sleep(self.random_sleep_seconds())
             else:
                 return
```

### Comparing `twitter_api_py-0.1.0/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py` & `twitter_api_py-0.2.0/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 from typing import Optional
 
 from twitter_api.rate_limit.manager.handlers.raise_rate_limit_handler import (
     RaiseRateLimitHandler,
 )
-from twitter_api.rate_limit.rate_limit_info import RateLimitInfo
+from twitter_api.rate_limit.types.rate_limit_info import RateLimitInfo
 
 
 class NoOperationRateLimitManager(RaiseRateLimitHandler):
     """
     レートリミットに関して、クライアント側で何も制御しないマネージャ。
 
     Twitter API がレートリミットエラーを返却ことを想定している。
```

### Comparing `twitter_api_py-0.1.0/twitter_api/rate_limit/manager/rate_limit_manager.py` & `twitter_api_py-0.2.0/twitter_api/rate_limit/manager/rate_limit_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABCMeta, abstractmethod
 from contextlib import asynccontextmanager, contextmanager
 from datetime import datetime
 from typing import AsyncGenerator, Generator, Optional
 
-from twitter_api.rate_limit.rate_limit_info import RateLimitInfo
+from twitter_api.rate_limit.types.rate_limit_info import RateLimitInfo
 
 
 class RateLimitManager(metaclass=ABCMeta):
     @abstractmethod
     def check_limit_over(
         self,
         rate_limit_info: RateLimitInfo,
@@ -16,27 +16,27 @@
         """
         レートリミットオーバーかを調べ、超えている場合は必要な待ち時間[秒]を返す。
         """
 
         ...
 
     @abstractmethod
-    @asynccontextmanager
-    async def handle_rate_limit_async(
+    @contextmanager
+    def handle_rate_limit_sync(
         self, rate_limit_info: RateLimitInfo
-    ) -> AsyncGenerator[None, None]:
+    ) -> Generator[None, None, None]:
         """
-        非同期的な TwitterApiAsyncClient を用いている場合のレートリミットの処理方法。
+        同期的な TwitterApiClient を用いている場合のレートリミットの対応方法。
         """
 
         yield
 
     @abstractmethod
-    @contextmanager
-    def handle_rate_limit_sync(
+    @asynccontextmanager
+    async def handle_rate_limit_async(
         self, rate_limit_info: RateLimitInfo
-    ) -> Generator[None, None, None]:
+    ) -> AsyncGenerator[None, None]:
         """
-        同期的な TwitterApiClient を用いている場合のレートリミットの処理方法。
+        非同期的な TwitterApiAsyncClient を用いている場合のレートリミットの対応方法。
         """
 
         yield
```

### Comparing `twitter_api_py-0.1.0/twitter_api/rate_limit/rate_limit.py` & `twitter_api_py-0.2.0/twitter_api/rate_limit/rate_limit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Callable, Literal, Optional, overload
 
 from twitter_api.api.resources.api_resources import ApiResources
 from twitter_api.client.request.request_async_client import RequestAsyncClient
-from twitter_api.error import RateLimitOverError
-from twitter_api.rate_limit.rate_limit_info import RateLimitInfo
-from twitter_api.rate_limit.rate_limit_target import RateLimitTarget
+from twitter_api.rate_limit.types.rate_limit_info import RateLimitInfo
+from twitter_api.rate_limit.types.rate_limit_target import RateLimitTarget
 from twitter_api.types.endpoint import Endpoint
 
 
 @overload
 def rate_limit(
     endpoint: Endpoint,
     target: RateLimitTarget,
```

### Comparing `twitter_api_py-0.1.0/twitter_api/types/comma_separatable.py` & `twitter_api_py-0.2.0/twitter_api/types/comma_separatable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional, TypeAlias, TypeVar, Union
 
 T = TypeVar("T", bound=str)
+
 CommaSeparatedStr: TypeAlias = str
 """
 要素がカンマ区切りで結合された文字列。
 """
 
 CommaSeparatable = Union[T, list[T]]
 """
```

### Comparing `twitter_api_py-0.1.0/twitter_api/types/extra_permissive_model.py` & `twitter_api_py-0.2.0/twitter_api/types/extra_permissive_model.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.1.0/twitter_api/types/http.py` & `twitter_api_py-0.2.0/twitter_api/types/http.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 
 @overload
 def downcast_dict(typed_dict: Optional[TypedDict]) -> Optional[dict]:
     ...
 
 
 def downcast_dict(typed_dict):
-    return typed_dict  # type: ignore
+    return typed_dict
```

### Comparing `twitter_api_py-0.1.0/twitter_api/types/model.py` & `twitter_api_py-0.2.0/twitter_api/types/model.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.1.0/twitter_api/types/oauth.py` & `twitter_api_py-0.2.0/twitter_api/types/oauth.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,38 +67,14 @@
 
 - Access secret
 - Access token secret
 - Token Secret
 - resulting oauth_token_secret
 """
 
-OAuthToken: TypeAlias = str
-"""
-OAuth 認証をするときに、一時的に発行されるトークン。
-
-同じことを指す用語として下記が存在する。
-- Request Token
-- oauth_token
-"""
-
-OAuthTokenSecret: TypeAlias = str
-"""
-OAuth 認証をするときに、一時的に発行されるトークンの秘密キー。
-
-同じことを指す用語として下記が存在する。
-- Request Token Secret
-- oauth_token_secret
-"""
-
-OauthVerifier: TypeAlias = str
-"""
-OAuth 認証をするときに、一時的に発行されるトークンを検証するキー。
-"""
-
-
 ClientId: TypeAlias = str
 """
 OAuth2.0 で認証をするときに必要なID。
 """
 
 ClientSecret: TypeAlias = str
 """
```

### Comparing `twitter_api_py-0.1.0/twitter_api/types/paging.py` & `twitter_api_py-0.2.0/twitter_api/types/paging.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,19 +7,21 @@
     Generator,
     Optional,
     Self,
     TypedDict,
     TypeVar,
 )
 
+from twitter_api.api.types.pagination_token import PaginationToken
+
 
 class PageResponseBody(metaclass=ABCMeta):
     @property
     @abstractmethod
-    def meta_next_token(self) -> Optional[str]:
+    def meta_next_token(self) -> Optional[PaginationToken]:
         ...
 
     @abstractmethod
     def extend(self, other: Self) -> None:
         ...
 
 
@@ -27,98 +29,102 @@
 
 AnyPageResponseBody = TypeVar(
     "AnyPageResponseBody",
     bound=PageResponseBody,
 )
 
 
-def get_paging_response_iter_sync(
+def get_paging_response_body_iter_sync(
     get_func: Callable[
         [AnyQueryParameters],
         AnyPageResponseBody,
     ],
     query: Optional[AnyQueryParameters],
+    pagination_token_key: str,
 ) -> Generator[AnyPageResponseBody, None, None]:
     """
     ページングされたレスポンスを返す API に対して、ページングをイテレータで返す。
     """
     if query is None:
-        _query: AnyQueryParameters = {"next_token": None}  # type: ignore
+        _query: AnyQueryParameters = {pagination_token_key: None}  # type: ignore
     else:
         _query = query
 
-    next_token = _query.get("next_token")
+    next_token = _query.get(pagination_token_key)
 
     while True:
-        _query["next_token"] = next_token  # type: ignore
-        response = get_func(_query)
+        _query[pagination_token_key] = next_token  # type: ignore
+        response_body = get_func(_query)
 
-        yield response
+        yield response_body
 
-        next_token = response.meta_next_token
+        next_token = response_body.meta_next_token
 
         if next_token is None:
             return
 
 
-def get_collected_paging_response_sync(
+def get_collected_paging_response_body_sync(
     get_func: Callable[
         [AnyQueryParameters],
         AnyPageResponseBody,
     ],
     query: Optional[AnyQueryParameters],
+    pagination_token_key: str,
 ) -> AnyPageResponseBody:
     """
     ページングされたレスポンスを返す API に対して、最後までデータを読み取り、結合した状態で返す。
     """
-    paging = get_paging_response_iter_sync(get_func, query)
+    paging = get_paging_response_body_iter_sync(get_func, query, pagination_token_key)
     first = next(paging)
 
     for page in paging:
         first.extend(page)
     return first
 
 
-async def get_paging_response_iter_async(
+async def get_paging_response_body_iter_async(
     get_func: Callable[
         [AnyQueryParameters],
         Coroutine[Any, Any, AnyPageResponseBody],
     ],
     query: Optional[AnyQueryParameters],
+    pagination_token_key: str,
 ) -> AsyncGenerator[AnyPageResponseBody, None]:
     """
     ページングされたレスポンスを返す API に対して、ページングをイテレータで返す。
     """
     if query is None:
-        _query: AnyQueryParameters = {"next_token": None}  # type: ignore
+        _query: AnyQueryParameters = {pagination_token_key: None}  # type: ignore
     else:
         _query = query
-    next_token = _query.get("next_token")
+    next_token = _query.get(pagination_token_key)
 
     while True:
-        _query["next_token"] = next_token  # type: ignore
-        response = await get_func(_query)
+        _query[pagination_token_key] = next_token  # type: ignore
+        response_body = await get_func(_query)
 
-        yield response
+        yield response_body
 
-        next_token = response.meta_next_token
+        next_token = response_body.meta_next_token
 
         if next_token is None:
             return
 
 
-async def get_collected_paging_response_async(
+async def get_collected_paging_response_body_async(
     get_func: Callable[
         [AnyQueryParameters],
         Coroutine[Any, Any, AnyPageResponseBody],
     ],
     query: Optional[AnyQueryParameters],
+    pagination_token_key: str,
 ) -> AnyPageResponseBody:
     """
     ページングされたレスポンスを返す API に対して、最後までデータを読み取り、結合した状態で返す。
     """
-    paging = get_paging_response_iter_async(get_func, query)
+    paging = get_paging_response_body_iter_async(get_func, query, pagination_token_key)
     first = await paging.__anext__()
 
     async for page in paging:
         first.extend(page)
     return first
```

### Comparing `twitter_api_py-0.1.0/twitter_api/utils/oauth.py` & `twitter_api_py-0.2.0/twitter_api/utils/_oauth.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 import re
 import string
 from time import time
 
 UNICODE_ASCII_CHARACTER_SET = string.ascii_letters + string.digits
 
 
-def generate_token(length=30, chars=UNICODE_ASCII_CHARACTER_SET):
+def generate_token(length=30, chars=UNICODE_ASCII_CHARACTER_SET) -> str:
     rand = random.SystemRandom()
     return "".join(rand.choice(chars) for _ in range(length))
 
 
-def generate_timestamp():
+def generate_timestamp() -> str:
     return str(int(time()))
 
 
 def generate_code_verifier() -> str:
     code_verifier = base64.urlsafe_b64encode(os.urandom(30)).decode("utf-8")
     return re.sub("[^a-zA-Z0-9]+", "", code_verifier)
```

### Comparing `twitter_api_py-0.1.0/twitter_api/warning.py` & `twitter_api_py-0.2.0/twitter_api/warning.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from twitter_api.error import TwitterApiException
-from twitter_api.rate_limit.rate_limit_info import RateLimitInfo
+from twitter_api.rate_limit.types.rate_limit_info import RateLimitInfo
 
 
 class TwitterApiWarning(TwitterApiException):
     ...
 
 
 class RateLimitOverWarning(TwitterApiWarning):
     def __init__(self, rate_limit: RateLimitInfo) -> None:
         self._rate_limit = rate_limit
 
-    def __str__(self) -> str:
+    @property
+    def message(self) -> str:
         return f"レートリミットを超えています。{self._rate_limit}"
 
 
 class UnmanagedRateLimitOverWarning(TwitterApiWarning):
-    def __str__(self) -> str:
+    @property
+    def message(self) -> str:
         return f"管理していないレートリミットに遭遇しました。"
```

### Comparing `twitter_api_py-0.1.0/PKG-INFO` & `twitter_api_py-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: twitter-api-py
-Version: 0.1.0
+Version: 0.2.0
 Summary: Twitter API Client by Typed Python.
+Home-page: https://github.com/yassun4dev/twitter-api-py
 License: BSD-3-Clause
 Author: yassun4dev
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -14,22 +15,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: authlib (>=1.2.0,<2.0.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Project-URL: Repository, https://github.com/yassun4dev/twitter-api-py
 Description-Content-Type: text/markdown
 
 # <p align="center">✨✨ Twitter API Client by Typed Python ✨✨</p>
 
 <p align="center">
     <a href="https://github.com/yassun4dev/twitter-api-py/actions">
         <img src="https://github.com/yassun4dev/twitter-api-py/actions/workflows/test-suite.yml/badge.svg" alt="Test Suite">
     </a>
+    <a href="https://pypi.org/project/twitter_api_py/">
+        <img src="https://badge.fury.io/py/twitter_api_py.svg" alt="Package version">
+    </a>
 </p>
 
 ![demo](https://raw.githubusercontent.com/yassun4dev/twitter-api-py/main/images/demo.gif)
 
 ## Install
 
 ```sh
@@ -43,30 +48,29 @@
 - Sync / Async Client support.
 - Mock Client support.
 
 
 ## Usage
 The simplest way to use the library is as follows:
 
-As a characteristic feature of the library, it explicitly prompts the user to write the Endpoint URL, which makes it clear from the source code which Twitter API is being called.
-
 ```python
 from twitter_api import TwitterApiClient
 
-twitter_client = TwitterApiClient.from_oauth2_app_env()
-
-response = (
-    twitter_client.resource("https://api.twitter.com/2/tweets")
-    .get({
-        "ids": "1460323737035677698",
-        "expansions": ["referenced_tweets.id"]
-    })
-)
+with TwitterApiClient.from_oauth2_app_env() as twitter_client:
+    response_body = (
+        twitter_client.request("https://api.twitter.com/2/tweets")
+        .get({
+            "ids": "1460323737035677698",
+            "expansions": ["referenced_tweets.id"]
+        })
+    )
 ```
 
+As a characteristic feature of the library, it explicitly prompts the user to write the Endpoint URL, which makes it clear from the source code which Twitter API is being called.
+
 ## Test Code
 
 A mock client is provided by the library to simplify the writing of test code.
 
 This client has the same interface as TwitterApiClient/TwitterApiAsyncClient, and also provides methods (`inject_*_response_body`) for injecting test data.
 
 ```python
@@ -75,17 +79,15 @@
 
 def your_logic(twitter_client: TwitterApiClient):
     ...
 
 def test_your_logic():
     twitter_client = (
         TwitterApiMockClient.from_oauth2_app_env()
-        .inject_post_response_body("https://api.twitter.com/2/tweets", post_response)
-        .inject_get_response_body("https://api.twitter.com/2/tweets/:id", get_response)
-        .inject_delete_response_body("https://api.twitter.com/2/tweets", delete_response)
+        .inject_post_response_body("https://api.twitter.com/2/tweets", post_response_body)
+        .inject_get_response_body("https://api.twitter.com/2/tweets/:id", get_response_body)
+        .inject_delete_response_body("https://api.twitter.com/2/tweets", delete_response_body)
     )
 
     assert your_logic(twitter_client) is True
 ```
 
-
-
```

