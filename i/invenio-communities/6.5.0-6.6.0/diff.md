# Comparing `tmp/invenio-communities-6.5.0.tar.gz` & `tmp/invenio-communities-6.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-communities-6.5.0.tar", last modified: Fri May  5 14:18:20 2023, max compression
+gzip compressed data, was "dist/invenio-communities-6.6.0.tar", last modified: Fri May 26 08:41:51 2023, max compression
```

## Comparing `invenio-communities-6.5.0.tar` & `invenio-communities-6.6.0.tar`

### file list

```diff
@@ -1,644 +1,644 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/.eslintrc.yml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/.prettierrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/administration/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/administration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/administration/communities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/alembic/5b478fe7ef7f_create_featured_communities_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/alembic/90642d415317_create_communities_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/alembic/a3f5a8635cbb_remove_version_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/alembic/de9c14cbb0b2_create_communities_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/alembic/f701a32e6fbe_create_communities_members_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/alembic/fbe746957cfc_create_member_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/FeatureModal.js
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/api.js
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/details.js
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/featured.js
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/search.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityApi.js
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityLinksExtractor.js
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/GroupsApi.js
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/UsersApi.js
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/InvitationsContextProvider.js
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/api.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/MembersContextProvider.js
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/api.js
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/serializers.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CarouselItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CommunitiesCarousel.js
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemComputer.js
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemMobile.js
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemComputer.js
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemMobile.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunities.js
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunity.js
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/frontpage.js
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/CommunityTypeLabel.js
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/RestrictedLabel.js
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/new.js
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/search.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesEmptySearchResults.js
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesResults.js
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchBarElement.js
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchLayout.js
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/ResultsGridItemTemplate.js
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/Filters.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ActionDropdown.js
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorMessage.js
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorPopup.js
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabel.js
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabels.js
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/MembersSearchBarElement.js
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/RemoveMemberModal.js
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/SuccessIcon.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/RadioSelection.js
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActions.js
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActionsManager.js
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsRowCheckbox.js
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SelectedMembers.js
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/context.js
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/dropdowns.js
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/ModalContextProvider.js
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/context.js
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/index.js
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationResultItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResults.js
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResultsContainer.js
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchBarElement.js
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchLayout.js
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/GroupTabPane.js
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/InvitationsMembersModal.js
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MemberSearchBar.js
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MembersWithRoleSelection.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/InvitationActionButtons.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersEmptyResults.js
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResult.js
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultContainer.js
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultsGridItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersSearchLayout.js
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMemberBulkActions.js
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultContainer.js
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultItem.js
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/MembersSearchAppContext.js
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultContainer.js
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersSearchLayout.js
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/requests.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/routes/appUrls.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/CommunitySettingsForm.js
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/CurationPolicyForm.js
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/CommunityPagesForm.js
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/CommunityPriviledgesForm.js
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/
--rw-r--r--   0 runner    (1001) docker     (123)    20359 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CommunityProfileForm.js
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CustomFieldSerializer.js
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DangerZone.js
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteButton.js
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteCommunityModal.js
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/LogoUploader.js
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/RenameCommunitySlugButton.js
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next-scanner.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/
--rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/
--rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/translations.json
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/translations.json
--rw-r--r--   0 runner    (1001) docker     (123)   130749 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/compileCatalog.js
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/initCatalog.js
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/translations.pot
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/communities/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/communities/dumpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/dumpers/featured.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/entity_resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/communities/records/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/communities/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/records/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/communities/records/jsonschemas/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/records/jsonschemas/communities/communities-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/records/jsonschemas/communities/definitions-v2.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/communities/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/communities/records/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/records/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/communities/records/mappings/os-v1/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/records/mappings/os-v1/communities/communities-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/communities/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/communities/records/mappings/os-v2/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/records/mappings/os-v2/communities/communities-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/communities/records/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/records/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/communities/records/mappings/v7/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/records/mappings/v7/communities/communities-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/communities/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/records/systemfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/records/systemfields/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/records/systemfields/pidslug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/communities/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/resources/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/resources/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/resources/ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/communities/services/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/services/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/services/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/services/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/services/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/services/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/services/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/communities/services/uow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/fixtures/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/fixtures/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/members/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/members/records/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v1/communitymembers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v1/communitymembers/members/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v1/communitymembers/members/member-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v2/communitymembers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v2/communitymembers/members/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v2/communitymembers/members/member-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/v7/communitymembers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/v7/communitymembers/members/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/records/mappings/v7/communitymembers/members/member-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/members/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/resources/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/members/services/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/services/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/services/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/services/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/services/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/services/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    23582 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/members/services/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/records/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/records/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/records/records/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/records/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/records/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/records/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/records/records/systemfields/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/records/records/systemfields/communities/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/records/records/systemfields/communities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/records/records/systemfields/communities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/records/records/systemfields/communities/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/records/records/systemfields/communities/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/searchapp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/administration/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/administration/community_details.html
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/administration/community_search.html
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/about/
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/about/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/access-status-label.html
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/custom_fields.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/invitations.html
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/members.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/curation_policy.html
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/pages.html
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/privileges.html
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/profile.html
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/communities_carousel.html
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/featured_communities.html
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/new.html
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/request.html
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/tombstone.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13804 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11074 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities/views/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/views/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11392 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/views/communities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/views/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/views/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/invenio_communities/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/invenio_communities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31716 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 14:18:19.000000 invenio-communities-6.5.0/invenio_communities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      698 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/run-js-linter.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1881 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/tests/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/communities/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/communities/test_alembic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/communities/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/communities/test_community_ui_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/communities/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/communities/test_relations_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/communities/test_relations_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26472 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/communities/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/communities/test_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/communities/tests_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/tests/members/
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/members/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/members/test_members_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/members/test_members_no_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/members/test_members_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    33612 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/members/test_members_services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/tests/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/records/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/tests/records/mock_module/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/records/mock_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/records/mock_module/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/tests/records/mock_module/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/records/mock_module/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/tests/records/mock_module/jsonschemas/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/records/mock_module/jsonschemas/mocks/mock-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/tests/records/mock_module/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/records/mock_module/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/tests/records/mock_module/mappings/v6/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/records/mock_module/mappings/v6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/tests/records/mock_module/mappings/v6/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/records/mock_module/mappings/v6/mocks/mock-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/tests/records/mock_module/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/records/mock_module/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:18:20.000000 invenio-communities-6.5.0/tests/records/mock_module/mappings/v7/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/records/mock_module/mappings/v7/mocks/mock-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/records/mock_module/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-05 14:18:10.000000 invenio-communities-6.5.0/tests/records/test_mockrecords_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/.eslintrc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/.prettierrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/administration/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/administration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/administration/communities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/alembic/5b478fe7ef7f_create_featured_communities_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/alembic/90642d415317_create_communities_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/alembic/a3f5a8635cbb_remove_version_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/alembic/de9c14cbb0b2_create_communities_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/alembic/f701a32e6fbe_create_communities_members_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/alembic/fbe746957cfc_create_member_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/FeatureModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/details.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/featured.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/search.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityApi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityLinksExtractor.js
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/GroupsApi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/UsersApi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/InvitationsContextProvider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/api.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/MembersContextProvider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/serializers.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CarouselItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CommunitiesCarousel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemComputer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemMobile.js
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemComputer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemMobile.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunities.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunity.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/frontpage.js
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/CommunityTypeLabel.js
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/RestrictedLabel.js
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/new.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/search.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesEmptySearchResults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesResults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchBarElement.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchLayout.js
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/ResultsGridItemTemplate.js
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/Filters.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ActionDropdown.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorMessage.js
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorPopup.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabels.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/MembersSearchBarElement.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/RemoveMemberModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/SuccessIcon.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/RadioSelection.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActionsManager.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsRowCheckbox.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SelectedMembers.js
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/context.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/dropdowns.js
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/ModalContextProvider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/context.js
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationResultItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResultsContainer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchBarElement.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchLayout.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/GroupTabPane.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/InvitationsMembersModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MemberSearchBar.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MembersWithRoleSelection.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/InvitationActionButtons.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersEmptyResults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResult.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultContainer.js
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultsGridItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersSearchLayout.js
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMemberBulkActions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultContainer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/MembersSearchAppContext.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultContainer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersSearchLayout.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/requests.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/routes/appUrls.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/CommunitySettingsForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/CurationPolicyForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/CommunityPagesForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/CommunityPriviledgesForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    20612 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CommunityProfileForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CustomFieldSerializer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DangerZone.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteButton.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteCommunityModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/LogoUploader.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/RenameCommunitySlugButton.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next-scanner.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/
+-rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)   130749 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/compileCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/initCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/translations.pot
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/communities/dumpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/dumpers/featured.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/entity_resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/communities/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/communities/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/records/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/communities/records/jsonschemas/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/records/jsonschemas/communities/communities-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/records/jsonschemas/communities/definitions-v2.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/communities/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/communities/records/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/records/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/communities/records/mappings/os-v1/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/records/mappings/os-v1/communities/communities-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/communities/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/communities/records/mappings/os-v2/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/records/mappings/os-v2/communities/communities-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/communities/records/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/records/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/communities/records/mappings/v7/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/records/mappings/v7/communities/communities-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/communities/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/records/systemfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/records/systemfields/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/records/systemfields/pidslug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/communities/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/resources/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/resources/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/resources/ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/communities/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/services/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/services/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/services/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/services/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/services/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/services/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/communities/services/uow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/fixtures/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/fixtures/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/members/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/members/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v1/communitymembers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v1/communitymembers/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v1/communitymembers/members/member-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v2/communitymembers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v2/communitymembers/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v2/communitymembers/members/member-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/v7/communitymembers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/v7/communitymembers/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/records/mappings/v7/communitymembers/members/member-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/members/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/resources/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/members/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/services/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/services/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/services/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/services/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/services/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23582 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/members/services/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/records/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/records/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/records/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/records/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/records/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/records/records/systemfields/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/records/records/systemfields/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/records/records/systemfields/communities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/records/records/systemfields/communities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/records/records/systemfields/communities/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/records/records/systemfields/communities/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/searchapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/administration/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/administration/community_details.html
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/administration/community_search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/about/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/about/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/access-status-label.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/custom_fields.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/invitations.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/members.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/curation_policy.html
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/pages.html
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/privileges.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/profile.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/communities_carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/featured_communities.html
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/request.html
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/tombstone.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13804 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11074 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/views/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/views/communities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/views/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/views/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/invenio_communities/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31716 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/invenio_communities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      698 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/run-js-linter.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1881 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/tests/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/communities/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/communities/test_alembic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/communities/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/communities/test_community_ui_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/communities/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/communities/test_relations_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/communities/test_relations_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29959 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/communities/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/communities/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/communities/tests_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/tests/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/members/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/members/test_members_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/members/test_members_no_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/members/test_members_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33612 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/members/test_members_services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/tests/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/records/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/tests/records/mock_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/records/mock_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/records/mock_module/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/tests/records/mock_module/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/records/mock_module/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/tests/records/mock_module/jsonschemas/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/records/mock_module/jsonschemas/mocks/mock-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/tests/records/mock_module/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/records/mock_module/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/tests/records/mock_module/mappings/v6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/records/mock_module/mappings/v6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/tests/records/mock_module/mappings/v6/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/records/mock_module/mappings/v6/mocks/mock-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/tests/records/mock_module/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/records/mock_module/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:41:51.000000 invenio-communities-6.6.0/tests/records/mock_module/mappings/v7/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/records/mock_module/mappings/v7/mocks/mock-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/records/mock_module/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-26 08:41:43.000000 invenio-communities-6.6.0/tests/records/test_mockrecords_api.py
```

### Comparing `invenio-communities-6.5.0/.editorconfig` & `invenio-communities-6.6.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/.tx/config` & `invenio-communities-6.6.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/AUTHORS.rst` & `invenio-communities-6.6.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/CHANGES.rst` & `invenio-communities-6.6.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,22 @@
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 
 Changes
 =======
 
+Version 6.6.0 (released 2023-05-26)
+-----------------------------------
+
+- configure number of items in communities carousel
+- add placeholder in communities carousel
+- introduce a configuration to disallow the creation of a restricted community
+- fix a11y for tabs and modals in communities settings
+
 Version 6.5.0 (released 2023-05-05)
 -----------------------------------
 
 - update mappings of members and invitations
 - add configurable community permission policy
 
 Version 6.4.0 (released 2023-04-25)
```

### Comparing `invenio-communities-6.5.0/CONTRIBUTING.rst` & `invenio-communities-6.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/LICENSE` & `invenio-communities-6.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/MANIFEST.in` & `invenio-communities-6.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/PKG-INFO` & `invenio-communities-6.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-communities
-Version: 6.5.0
+Version: 6.6.0
 Summary: InvenioRDM module for the communities feature.
 Home-page: https://github.com/inveniosoftware/invenio-communities
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -45,14 +45,22 @@
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         
         Changes
         =======
         
+        Version 6.6.0 (released 2023-05-26)
+        -----------------------------------
+        
+        - configure number of items in communities carousel
+        - add placeholder in communities carousel
+        - introduce a configuration to disallow the creation of a restricted community
+        - fix a11y for tabs and modals in communities settings
+        
         Version 6.5.0 (released 2023-05-05)
         -----------------------------------
         
         - update mappings of members and invitations
         - add configurable community permission policy
         
         Version 6.4.0 (released 2023-04-25)
```

### Comparing `invenio-communities-6.5.0/README.rst` & `invenio-communities-6.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/docs/Makefile` & `invenio-communities-6.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/docs/conf.py` & `invenio-communities-6.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/docs/index.rst` & `invenio-communities-6.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/docs/make.bat` & `invenio-communities-6.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/administration/communities.py` & `invenio-communities-6.6.0/invenio_communities/administration/communities.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/alembic/5b478fe7ef7f_create_featured_communities_table.py` & `invenio-communities-6.6.0/invenio_communities/alembic/5b478fe7ef7f_create_featured_communities_table.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/alembic/90642d415317_create_communities_branch.py` & `invenio-communities-6.6.0/invenio_communities/alembic/90642d415317_create_communities_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/alembic/a3f5a8635cbb_remove_version_table.py` & `invenio-communities-6.6.0/invenio_communities/alembic/a3f5a8635cbb_remove_version_table.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/alembic/de9c14cbb0b2_create_communities_tables.py` & `invenio-communities-6.6.0/invenio_communities/alembic/de9c14cbb0b2_create_communities_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/alembic/f701a32e6fbe_create_communities_members_table.py` & `invenio-communities-6.6.0/invenio_communities/alembic/f701a32e6fbe_create_communities_members_table.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/alembic/fbe746957cfc_create_member_tables.py` & `invenio-communities-6.6.0/invenio_communities/alembic/fbe746957cfc_create_member_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/FeatureModal.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/FeatureModal.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -96,29 +96,33 @@
                 Header as = "h2" > {
                     i18next.t("Planned features")
                 } < /Header> {
                     loading && < Loader active = {
                         loading
                     }
                     />} {
-                        error && < ErrorMessage error = {
+                        error && < ErrorMessage id = "featured-community-errors"
+                        error = {
                             error
                         }
                         />} {
                             !loading && !error && ( <
                                 Table celled striped collapsing >
                                 <
                                 Table.Header >
                                 <
+                                Table.Row >
+                                <
                                 Table.HeaderCell > {
                                     i18next.t("Start date")
                                 } < /Table.HeaderCell> <
                                 Table.HeaderCell > {
                                     i18next.t("Active")
                                 } < /Table.HeaderCell> <
+                                /Table.Row> <
                                 /Table.Header> <
                                 Table.Body > {
                                     featuredList?.hits?.hits.map((row) => {
                                         const startDate = DateTime.fromISO(row.start_date);
                                         return ( <
                                             Table.Row key = {
                                                 row.id
```

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/details.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/details.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/featured.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/featured.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/search.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/search.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityApi.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityApi.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityLinksExtractor.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityLinksExtractor.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/InvitationsContextProvider.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/InvitationsContextProvider.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/api.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/api.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/MembersContextProvider.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/MembersContextProvider.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/api.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/api.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/serializers.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/serializers.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CarouselItem.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CarouselItem.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/index.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/index.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -15,14 +15,15 @@
 
 const communitiesCarouselContainer = document.getElementById("communities-carousel");
 const title = communitiesCarouselContainer.dataset.title;
 const fetchUrl = communitiesCarouselContainer.dataset.fetchUrl;
 const intervalDelay = parseInt(communitiesCarouselContainer.dataset.intervalDelay);
 const animationSpeed = parseInt(communitiesCarouselContainer.dataset.animationSpeed);
 const defaultLogo = communitiesCarouselContainer.dataset.defaultLogo;
+const itemsPerPage = communitiesCarouselContainer.dataset.itemsPerPage;
 
 const overriddenComponents = overrideStore.getAll();
 
 ReactDOM.render( <
     OverridableContext.Provider value = {
         overriddenComponents
     } >
@@ -38,11 +39,14 @@
     }
     animationSpeed = {
         animationSpeed
     }
     defaultLogo = {
         defaultLogo
     }
+    itemsPerPage = {
+        itemsPerPage
+    }
     /> <
     /OverridableContext.Provider>,
     communitiesCarouselContainer
 );
```

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItem.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItem.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,16 @@
     CommunityCompactItemMobile
 } from "./CommunityCompactItemMobile";
 
 export function CommunityCompactItem({
     result,
     actions,
     extraLabels,
-    itemClassName
+    itemClassName,
+    showPermissionLabel,
 }) {
     return ( <
         >
         <
         CommunityCompactItemComputer result = {
             result
         }
@@ -25,14 +26,17 @@
         }
         extraLabels = {
             extraLabels
         }
         itemClassName = {
             itemClassName
         }
+        showPermissionLabel = {
+            showPermissionLabel
+        }
         /> <
         CommunityCompactItemMobile result = {
             result
         }
         actions = {
             actions
         }
@@ -48,14 +52,16 @@
 }
 
 CommunityCompactItem.propTypes = {
     result: PropTypes.object.isRequired,
     actions: PropTypes.node,
     extraLabels: PropTypes.node,
     itemClassName: PropTypes.string,
+    showPermissionLabel: PropTypes.bool,
 };
 
 CommunityCompactItem.defaultProps = {
     actions: undefined,
     extraLabels: undefined,
     itemClassName: "",
+    showPermissionLabel: false,
 };
```

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemComputer.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemMobile.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,124 +1,140 @@
 // This file is part of InvenioRDM
-// Copyright (C) 2023 CERN.
+// Copyright (C) 2022 CERN.
 //
-// InvenioRDM is free software; you can redistribute it and/or modify it
+// Invenio App RDM is free software; you can redistribute it and/or modify it
 // under the terms of the MIT License; see LICENSE file for more details.
 
-import _truncate from "lodash/truncate";
-import PropTypes from "prop-types";
-import React from "react";
+import {
+    i18next
+} from "@translations/invenio_app_rdm/i18next";
 import {
     CommunityTypeLabel
 } from "../labels";
-
 import {
-    Grid,
-    Container,
-    Image,
+    RestrictedLabel
+} from "../labels";
+import React from "react";
+import {
+    Image
+} from "react-invenio-forms";
+import {
+    Button,
     Item
 } from "semantic-ui-react";
+import PropTypes from "prop-types";
 import {
-    RestrictedLabel
-} from "../labels";
+    DateTime
+} from "luxon";
 
-export const CommunityCompactItemComputer = ({
+export const CommunityItemMobile = ({
     result,
-    actions,
-    extraLabels,
-    itemClassName,
+    index
 }) => {
-    const {
-        metadata,
-        links,
-        access,
-        id
-    } = result;
-    const ui = result.ui;
-
-    const communityType = ui?.type?.title_l10n;
+    const communityType = result.ui?.type?.title_l10n;
 
     return ( <
         Item key = {
-            id
-        }
-        className = {
-            `computer tablet only justify-space-between community-item ${itemClassName}`
-        } >
-        <
-        Image as = {
-            Item.Image
-        }
-        size = "tiny"
-        src = {
-            links.logo
+            index
         }
-        /> <
-        Grid >
-        <
-        Grid.Column width = {
-            10
-        } >
+        className = "mobile only community-item" >
         <
-        Item.Content verticalAlign = "middle" >
+        Item.Content className = "centered" >
         <
-        Item.Header as = "h3"
-        className = "ui small header flex align-items-center mb-5" >
+        Item.Extra className = "user-communities" >
         <
-        a href = {
-            links.self_html
+        RestrictedLabel access = {
+            result.access.visibility
         }
-        className = "p-0" > {
-            metadata.title
-        } <
-        /a> <
-        /Item.Header>
-
-        <
-        Item.Description >
-        <
-        div dangerouslySetInnerHTML = {
-            {
-                __html: _truncate(metadata.description, {
-                    length: 50
-                }),
-            }
+        /> <
+        CommunityTypeLabel type = {
+            communityType
         }
         /> <
-        /Item.Description> <
+        /Item.Extra> <
         Item.Extra >
         <
-        RestrictedLabel access = {
-            access.visibility
+        Image wrapped src = {
+            result.links.logo
         }
-        /> <
-        CommunityTypeLabel type = {
-            communityType
+        size = "small"
+        alt = "" / >
+        <
+        /Item.Extra> <
+        Item.Header as = "h2"
+        className = "rel-mt-1 mb-10" >
+        <
+        a href = {
+            result.links.self_html
+        } > {
+            result.metadata.title
+        } < /a> <
+        /Item.Header>
+
+        {
+            result.metadata.description && ( <
+                Item.Description as = "p"
+                className = "truncate-lines-2 mb-10"
+                dangerouslySetInnerHTML = {
+                    {
+                        __html: result.metadata.description,
+                    }
+                }
+                />
+            )
+        }
+
+        {
+            result.metadata.website && ( <
+                Item.Meta className = "mb-10" > {
+                    result.metadata.website && ( <
+                        a href = {
+                            result.metadata.website
+                        }
+                        target = "_blank"
+                        rel = "noopener noreferrer" >
+                        {
+                            result.metadata.website
+                        } <
+                        /a>
+                    )
+                } <
+                /Item.Meta>
+            )
         }
-        /> {
-            extraLabels
+
+        <
+        Item.Extra className = "mb-10" > {
+            i18next.t("Created: ")
+        } {
+            DateTime.fromISO(result.created).toLocaleString(i18next.language)
+        } <
+        /Item.Extra> {
+            result.ui.permissions.can_update && ( <
+                Item.Extra >
+                <
+                Button compact size = "small"
+                fluid href = {
+                    result.links.settings_html
+                }
+                labelPosition = "left"
+                icon = "edit"
+                content = {
+                    i18next.t("Edit")
+                }
+                /> <
+                /Item.Extra>
+            )
         } <
-        /Item.Extra> <
         /Item.Content> <
-        /Grid.Column> <
-        /Grid> <
-        Container fluid >
-        <
-        div className = "flex flex-direction-column align-items-end" > {
-            actions
-        } < /div> <
-        /Container> <
         /Item>
     );
 };
-CommunityCompactItemComputer.propTypes = {
+
+CommunityItemMobile.propTypes = {
     result: PropTypes.object.isRequired,
-    actions: PropTypes.node,
-    extraLabels: PropTypes.node,
-    itemClassName: PropTypes.string,
+    index: PropTypes.string,
 };
 
-CommunityCompactItemComputer.defaultProps = {
-    actions: undefined,
-    extraLabels: undefined,
-    itemClassName: "",
+CommunityItemMobile.defaultProps = {
+    index: null,
 };
```

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemMobile.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemMobile.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -32,57 +32,62 @@
         }
         className = "mobile only justify-space-between" >
         <
         Image size = "mini"
         src = {
             result.links.logo
         }
-        />
+        alt = "" / >
 
         <
         Item.Content verticalAlign = "middle" >
         <
-        Item.Header as = "h3"
-        className = "ui small header flex align-items-center mb-5" >
-        <
-        a href = {
+        Item.Header as = "a"
+        href = {
             result.links.self_html
         }
-        className = "p-0" > {
+        className = "ui small header flex align-items-center mb-5" >
+        {
             result.metadata.title
         } <
-        /a> <
         /Item.Header>
 
-        <
-        Item.Description dangerouslySetInnerHTML = {
-            {
-                __html: _truncate(result.metadata.description, {
-                    length: 50
-                }),
-            }
+        {
+            result.metadata.description && ( <
+                Item.Description as = "p"
+                dangerouslySetInnerHTML = {
+                    {
+                        __html: _truncate(result.metadata.description, {
+                            length: 50
+                        }),
+                    }
+                }
+                />
+            )
         }
-        /> <
+
+        <
         Item.Extra >
         <
         RestrictedLabel access = {
             result.access.visibility
         }
         /> <
         CommunityTypeLabel type = {
             communityType
         }
         /> <
         /Item.Extra> <
         /Item.Content>
 
         <
-        div className = "flex align-items-start" > {
+        div className = "flex flex-direction-column align-items-center rel-mt-1" > {
             actions
-        } < /div> <
+        } <
+        /div> <
         /Item>
     );
 };
 
 CommunityCompactItemMobile.propTypes = {
     result: PropTypes.object.isRequired,
     actions: PropTypes.node,
```

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemComputer.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemComputer.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -41,15 +41,16 @@
         <
         Image as = {
             Item.Image
         }
         wrapped src = {
             result.links.logo
         }
-        className = "community-logo" /
+        className = "community-logo"
+        alt = "" /
         >
         <
         Grid >
         <
         Grid.Column width = {
             12
         } >
@@ -62,37 +63,45 @@
         } >
         <
         a href = {
             result.links.self_html
         } > {
             result.metadata.title
         } < /a> <
-        /Item.Header> <
-        Item.Meta >
-        <
-        a href = {
-            result.metadata.website
+        /Item.Header>
+
+        {
+            result.metadata.website && ( <
+                Item.Meta >
+                <
+                a href = {
+                    result.metadata.website
+                }
+                target = "_blank"
+                rel = "noopener noreferrer" >
+                {
+                    result.metadata.website
+                } <
+                /a> <
+                /Item.Meta>
+            )
         }
-        target = "_blank"
-        rel = "noopener noreferrer" >
+
         {
-            result.metadata.website
-        } <
-        /a> <
-        /Item.Meta> <
-        Item.Description >
-        <
-        div className = "truncate-lines-2"
-        dangerouslySetInnerHTML = {
-            {
-                __html: result.metadata.description,
-            }
+            result.metadata.description && ( <
+                Item.Description as = "p"
+                className = "truncate-lines-2"
+                dangerouslySetInnerHTML = {
+                    {
+                        __html: result.metadata.description,
+                    }
+                }
+                />
+            )
         }
-        /> <
-        /Item.Description>
 
         <
         Item.Extra >
         <
         RestrictedLabel access = {
             result.access.visibility
         }
```

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunities.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunities.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunity.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunity.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/index.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/frontpage.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/frontpage.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/index.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/RestrictedLabel.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/RestrictedLabel.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/new.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/new.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -142,15 +142,16 @@
                 }) => setFieldError(field, messages[0]));
             }
         }
     };
 
     render() {
         const {
-            formConfig
+            formConfig,
+            canCreateRestricted
         } = this.props;
         const {
             error
         } = this.state;
 
         return ( <
             Formik initialValues = {
@@ -266,57 +267,63 @@
                                     (widget) => import(`@templates/custom_fields/${widget}.js`),
                                     (widget) => import(`react-invenio-forms`),
                                 ]
                             }
                             fieldPathPrefix = "custom_fields" /
                             >
                         )
-                    } <
-                    Header as = "h3" > {
-                        i18next.t("Community visibility")
-                    } < /Header> {
-                        formConfig.access.visibility.map((item) => ( <
-                            React.Fragment key = {
-                                item.value
-                            } >
+                    } {
+                        canCreateRestricted && ( <
+                            >
                             <
-                            RadioField key = {
-                                item.value
-                            }
-                            fieldPath = "access.visibility"
-                            label = {
-                                item.text
-                            }
-                            labelIcon = {
-                                item.icon
-                            }
-                            checked = {
-                                _get(values, "access.visibility") === item.value
-                            }
-                            value = {
-                                item.value
-                            }
-                            onChange = {
-                                ({
-                                    event,
-                                    data,
-                                    formikProps
-                                }) => {
-                                    formikProps.form.setFieldValue(
-                                        "access.visibility",
+                            Header as = "h3" > {
+                                i18next.t("Community visibility")
+                            } < /Header> {
+                                formConfig.access.visibility.map((item) => ( <
+                                    React.Fragment key = {
                                         item.value
-                                    );
-                                }
-                            }
-                            /> <
-                            label className = "helptext" > {
-                                item.helpText
-                            } < /label> <
-                            /React.Fragment>
-                        ))
+                                    } >
+                                    <
+                                    RadioField key = {
+                                        item.value
+                                    }
+                                    fieldPath = "access.visibility"
+                                    label = {
+                                        item.text
+                                    }
+                                    labelIcon = {
+                                        item.icon
+                                    }
+                                    checked = {
+                                        _get(values, "access.visibility") === item.value
+                                    }
+                                    value = {
+                                        item.value
+                                    }
+                                    onChange = {
+                                        ({
+                                            event,
+                                            data,
+                                            formikProps
+                                        }) => {
+                                            formikProps.form.setFieldValue(
+                                                "access.visibility",
+                                                item.value
+                                            );
+                                        }
+                                    }
+                                    /> <
+                                    label className = "helptext" > {
+                                        item.helpText
+                                    } < /label> <
+                                    /React.Fragment>
+                                ))
+                            } <
+                            />
+                        )
                     } <
                     /Grid.Column> <
                     /Grid.Row> <
                     Grid.Row >
                     <
                     Grid.Column textAlign = "center" >
                     <
@@ -345,24 +352,29 @@
             /Formik>
         );
     }
 }
 
 CommunityCreateForm.propTypes = {
     formConfig: PropTypes.object.isRequired,
+    canCreateRestricted: PropTypes.bool.isRequired,
 };
 
 const domContainer = document.getElementById("app");
 const formConfig = JSON.parse(domContainer.dataset.formConfig);
 const customFields = JSON.parse(domContainer.dataset.customFields);
+const canCreateRestricted = JSON.parse(domContainer.dataset.canCreateRestricted);
 
 ReactDOM.render( <
     CommunityCreateForm formConfig = {
         formConfig
     }
     customFields = {
         customFields
     }
+    canCreateRestricted = {
+        canCreateRestricted
+    }
     />,
     domContainer
 );
 export default CommunityCreateForm;
```

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/search.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/search.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesEmptySearchResults.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesEmptySearchResults.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesResults.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesResults.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchBarElement.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchBarElement.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchLayout.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchLayout.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/ResultsGridItemTemplate.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/ResultsGridItemTemplate.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/Filters.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/Filters.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ActionDropdown.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ActionDropdown.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorMessage.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorMessage.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorPopup.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorPopup.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabel.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabel.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabels.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabels.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/MembersSearchBarElement.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/MembersSearchBarElement.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/RemoveMemberModal.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/RemoveMemberModal.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/SuccessIcon.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/SuccessIcon.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/RadioSelection.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/RadioSelection.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActions.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActions.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActionsManager.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActionsManager.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsRowCheckbox.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsRowCheckbox.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SelectedMembers.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SelectedMembers.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/dropdowns.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/dropdowns.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/ModalContextProvider.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/ModalContextProvider.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationResultItem.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationResultItem.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResults.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResults.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResultsContainer.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResultsContainer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchBarElement.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchBarElement.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchLayout.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchLayout.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/index.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/GroupTabPane.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/GroupTabPane.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/InvitationsMembersModal.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/InvitationsMembersModal.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MemberSearchBar.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MemberSearchBar.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MembersWithRoleSelection.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MembersWithRoleSelection.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/InvitationActionButtons.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/InvitationActionButtons.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersEmptyResults.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersEmptyResults.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResult.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResult.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultContainer.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultContainer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultsGridItem.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultsGridItem.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersSearchLayout.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersSearchLayout.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMemberBulkActions.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMemberBulkActions.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultContainer.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultContainer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultItem.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultItem.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/MembersSearchAppContext.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/MembersSearchAppContext.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/index.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/index.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultContainer.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultContainer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultItem.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultItem.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersSearchLayout.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersSearchLayout.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/index.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/index.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/requests.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/requests.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/CommunitySettingsForm.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/CommunitySettingsForm.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/CurationPolicyForm.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/CurationPolicyForm.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/CommunityPagesForm.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/CommunityPagesForm.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/CommunityPriviledgesForm.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/CommunityPriviledgesForm.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CommunityProfileForm.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CommunityProfileForm.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -422,15 +422,16 @@
                     /Grid.Column> <
                     /Grid> <
                     /Message> <
                     Grid >
                     <
                     Grid.Row >
                     <
-                    Grid.Column mobile = {
+                    Grid.Column as = "section"
+                    mobile = {
                         16
                     }
                     tablet = {
                         10
                     }
                     computer = {
                         11
@@ -712,15 +713,16 @@
                     } >
                     <
                     Icon name = "save" / > {
                         i18next.t("Save")
                     } <
                     /Button> <
                     /Grid.Column> <
-                    Grid.Column mobile = {
+                    Grid.Column as = "section"
+                    mobile = {
                         16
                     }
                     tablet = {
                         5
                     }
                     computer = {
                         4
@@ -743,15 +745,16 @@
                         logoMaxSize
                     }
                     /> <
                     /Grid.Column> <
                     /Grid.Row> <
                     Grid.Row className = "danger-zone" >
                     <
-                    Grid.Column width = {
+                    Grid.Column as = "section"
+                    width = {
                         16
                     } >
                     <
                     DangerZone community = {
                         community
                     }
                     onError = {
```

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CustomFieldSerializer.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CustomFieldSerializer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DangerZone.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DangerZone.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteButton.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteButton.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteCommunityModal.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteCommunityModal.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/LogoUploader.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/LogoUploader.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -108,17 +108,20 @@
                     ...getRootProps()
                 } >
                 <
                 input {
                     ...getInputProps()
                 }
                 /> <
-                Header className = "mt-0" > {
+                Header as = "h2"
+                size = "small"
+                className = "mt-0" > {
                     i18next.t("Profile picture")
-                } < /Header> <
+                } <
+                /Header> <
                 Image src = {
                     logoURL
                 }
                 fallbackSrc = {
                     defaultLogo
                 }
                 loadFallbackFirst fluid wrapped rounded className = "community-logo settings" /
```

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/RenameCommunitySlugButton.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/RenameCommunitySlugButton.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -37,27 +37,35 @@
         this.state = {
             modalOpen: false,
             loading: false,
             error: "",
         };
 
         this.formInputRef = React.createRef();
+        this.modalTriggerRef = React.createRef();
+    }
+
+    componentDidUpdate() {
+        this.formInputRef.current && this.formInputRef.current.focus();
     }
 
     componentWillUnmount() {
         this.cancellableRename && this.cancellableRename.cancel();
     }
 
     handleOpen = () => this.setState({
         modalOpen: true
     });
 
-    handleClose = () => this.setState({
-        modalOpen: false
-    });
+    handleClose = () => {
+        this.setState({
+            modalOpen: false
+        });
+        this.modalTriggerRef.current.focus();
+    };
 
     handleChange = async (event) => {
         // stop event propagation so the submit event is restricted to the modal
         // form
         event.stopPropagation();
         const {
             community
@@ -87,29 +95,33 @@
             if (errors) {
                 const invalidIdError = errors
                     .filter((error) => error.field === "slug")
                     .map((error) => error.messages[0]);
                 this.setState({
                     error: invalidIdError
                 });
+                this.formInputRef.current.focus();
             }
         }
     };
 
     render() {
         const {
             modalOpen,
             loading,
             error
         } = this.state;
 
         return ( <
             >
             <
-            Button compact negative onClick = {
+            Button ref = {
+                this.modalTriggerRef
+            }
+            compact negative onClick = {
                 this.handleOpen
             }
             fluid icon labelPosition = "left"
             type = "button" >
             <
             Icon name = "pencil" / > {
                 i18next.t("Change identifier")
```

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/index.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next-scanner.config.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next-scanner.config.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/index.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/messages.po` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/translations.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package-lock.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package-lock.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package.json` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/compileCatalog.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/compileCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/initCatalog.js` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/initCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/translations.pot` & `invenio-communities-6.6.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/translations.pot`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/cli.py` & `invenio-communities-6.6.0/invenio_communities/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/__init__.py` & `invenio-communities-6.6.0/invenio_communities/communities/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/dumpers/featured.py` & `invenio-communities-6.6.0/invenio_communities/communities/dumpers/featured.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/entity_resolvers.py` & `invenio-communities-6.6.0/invenio_communities/communities/entity_resolvers.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/records/api.py` & `invenio-communities-6.6.0/invenio_communities/communities/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/records/jsonschemas/communities/communities-v1.0.0.json` & `invenio-communities-6.6.0/invenio_communities/communities/records/jsonschemas/communities/communities-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/records/jsonschemas/communities/definitions-v2.0.0.json` & `invenio-communities-6.6.0/invenio_communities/communities/records/jsonschemas/communities/definitions-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/records/mappings/os-v1/communities/communities-v1.0.0.json` & `invenio-communities-6.6.0/invenio_communities/communities/records/mappings/os-v1/communities/communities-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/records/mappings/os-v2/communities/communities-v1.0.0.json` & `invenio-communities-6.6.0/invenio_communities/communities/records/mappings/os-v2/communities/communities-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/records/mappings/v7/communities/communities-v1.0.0.json` & `invenio-communities-6.6.0/invenio_communities/communities/records/mappings/v7/communities/communities-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/records/models.py` & `invenio-communities-6.6.0/invenio_communities/communities/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/records/systemfields/access.py` & `invenio-communities-6.6.0/invenio_communities/communities/records/systemfields/access.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/records/systemfields/pidslug.py` & `invenio-communities-6.6.0/invenio_communities/communities/records/systemfields/pidslug.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/resources/config.py` & `invenio-communities-6.6.0/invenio_communities/communities/resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/resources/resource.py` & `invenio-communities-6.6.0/invenio_communities/communities/resources/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/resources/serializer.py` & `invenio-communities-6.6.0/invenio_communities/communities/resources/serializer.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/resources/ui_schema.py` & `invenio-communities-6.6.0/invenio_communities/communities/resources/ui_schema.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/schema.py` & `invenio-communities-6.6.0/invenio_communities/communities/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/services/__init__.py` & `invenio-communities-6.6.0/invenio_communities/communities/services/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/services/components.py` & `invenio-communities-6.6.0/invenio_communities/communities/services/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     RelationsComponent,
     ServiceComponent,
 )
 from marshmallow.exceptions import ValidationError
 
 from ...proxies import current_roles
 from ...utils import on_membership_change
+from ..records.systemfields.access import VisibilityEnum
 
 
 class PIDComponent(ServiceComponent):
     """Service component for Community PIDs."""
 
     def set_slug(self, record, slug):
         """Set slug."""
@@ -65,20 +66,38 @@
 
 
 class CommunityAccessComponent(ServiceComponent):
     """Service component for access integration."""
 
     def _populate_access_and_validate(self, identity, data, record, **kwargs):
         """Populate and validate the community's access field."""
-        if record is not None and "access" in data:
-            # populate the record's access field with the data already
-            # validated by marshmallow
-            record.setdefault("access", {})
-            record["access"].update(data.get("access", {}))
-            record.access.refresh_from_dict(record.get("access"))
+        is_modifying_access = record is not None and "access" in data
+
+        if not is_modifying_access:
+            return
+
+        access = data.get("access", {})
+        new_visibility = access.get("visibility")
+
+        record_has_defined_access = "access" in record
+        is_restricting = new_visibility == "restricted"
+
+        if (
+            VisibilityEnum(record.access.visibility) != new_visibility
+            and record_has_defined_access
+        ):
+            self.service.require_permission(identity, "manage_access", record=record)
+        if not record_has_defined_access and is_restricting:
+            self.service.require_permission(
+                identity, "create_restricted", record=record
+            )
+
+        record.setdefault("access", {})
+        record["access"].update(access)
+        record.access.refresh_from_dict(record.get("access"))
 
     def create(self, identity, data=None, record=None, **kwargs):
         """Add basic ownership fields to the record."""
         self._populate_access_and_validate(identity, data, record, **kwargs)
 
     def update(self, identity, data=None, record=None, **kwargs):
         """Update handler."""
```

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/services/config.py` & `invenio-communities-6.6.0/invenio_communities/communities/services/config.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/services/facets.py` & `invenio-communities-6.6.0/invenio_communities/communities/services/facets.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/services/links.py` & `invenio-communities-6.6.0/invenio_communities/communities/services/links.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/services/results.py` & `invenio-communities-6.6.0/invenio_communities/communities/services/results.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/services/service.py` & `invenio-communities-6.6.0/invenio_communities/communities/services/service.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/services/sort.py` & `invenio-communities-6.6.0/invenio_communities/communities/services/sort.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/communities/services/uow.py` & `invenio-communities-6.6.0/invenio_communities/communities/services/uow.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/config.py` & `invenio-communities-6.6.0/invenio_communities/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,7 +289,9 @@
         },
         ...
     }]
 """
 
 # Preview: Feature flag for invenio-app-rdm v11
 COMMUNITIES_ADMINISTRATION_DISABLED = True
+
+COMMUNITIES_ALLOW_RESTRICTED = True
```

### Comparing `invenio-communities-6.5.0/invenio_communities/errors.py` & `invenio-communities-6.6.0/invenio_communities/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/ext.py` & `invenio-communities-6.6.0/invenio_communities/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/fixtures/demo.py` & `invenio-communities-6.6.0/invenio_communities/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/fixtures/tasks.py` & `invenio-communities-6.6.0/invenio_communities/fixtures/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/generators.py` & `invenio-communities-6.6.0/invenio_communities/generators.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Community permissions."""
 
 import operator
+from abc import abstractmethod
 from collections import namedtuple
 from functools import partial, reduce
 from itertools import chain
 
 from flask import current_app
 from flask_principal import UserNeed
 from invenio_access.permissions import any_user, system_process
@@ -307,7 +308,61 @@
             for m in member_types:
                 if (
                     m in self.need_groups_enabled_types
                     and not current_app.config["COMMUNITIES_GROUPS_ENABLED"]
                 ):
                     return [any_user]
         return []
+
+
+# TODO https://github.com/inveniosoftware/invenio-rdm-records/issues/1226
+class ConditionalGenerator(Generator):
+    """Generator that depends on whether a condition is true or not.
+
+    If...(
+        then_=[...],
+        else_=[...],
+    )
+    """
+
+    def __init__(self, then_, else_):
+        """Constructor."""
+        self.then_ = then_
+        self.else_ = else_
+
+    @abstractmethod
+    def _condition(self, **kwargs):
+        """Condition to choose generators set."""
+        raise NotImplementedError()
+
+    def _generators(self, record, **kwargs):
+        """Get the "then" or "else" generators."""
+        return self.then_ if self._condition(record=record, **kwargs) else self.else_
+
+    def needs(self, record=None, **kwargs):
+        """Set of Needs granting permission."""
+        needs = [
+            g.needs(record=record, **kwargs) for g in self._generators(record, **kwargs)
+        ]
+        return set(chain.from_iterable(needs))
+
+    def excludes(self, record=None, **kwargs):
+        """Set of Needs denying permission."""
+        excludes = [
+            g.excludes(record=record, **kwargs)
+            for g in self._generators(record, **kwargs)
+        ]
+        return set(chain.from_iterable(excludes))
+
+
+class IfConfig(ConditionalGenerator):
+    """Config-based conditional generator."""
+
+    def __init__(self, config_key, accept_values=[True], **kwargs):
+        """Initialize generator."""
+        self.accept_values = accept_values
+        self.config_key = config_key
+        super().__init__(**kwargs)
+
+    def _condition(self, **_):
+        """Check if the config value is truthy."""
+        return current_app.config.get(self.config_key) in self.accept_values
```

### Comparing `invenio-communities-6.5.0/invenio_communities/members/__init__.py` & `invenio-communities-6.6.0/invenio_communities/members/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/errors.py` & `invenio-communities-6.6.0/invenio_communities/members/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/records/api.py` & `invenio-communities-6.6.0/invenio_communities/members/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json` & `invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v1/communitymembers/members/member-v1.0.0.json` & `invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v1/communitymembers/members/member-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json` & `invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/records/mappings/os-v2/communitymembers/members/member-v1.0.0.json` & `invenio-communities-6.6.0/invenio_communities/members/records/mappings/os-v2/communitymembers/members/member-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json` & `invenio-communities-6.6.0/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/records/mappings/v7/communitymembers/members/member-v1.0.0.json` & `invenio-communities-6.6.0/invenio_communities/members/records/mappings/v7/communitymembers/members/member-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/records/models.py` & `invenio-communities-6.6.0/invenio_communities/members/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/resources/config.py` & `invenio-communities-6.6.0/invenio_communities/members/resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/resources/resource.py` & `invenio-communities-6.6.0/invenio_communities/members/resources/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/services/components.py` & `invenio-communities-6.6.0/invenio_communities/members/services/components.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/services/config.py` & `invenio-communities-6.6.0/invenio_communities/members/services/config.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/services/facets.py` & `invenio-communities-6.6.0/invenio_communities/members/services/facets.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/services/fields.py` & `invenio-communities-6.6.0/invenio_communities/members/services/fields.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/services/request.py` & `invenio-communities-6.6.0/invenio_communities/members/services/request.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/services/schemas.py` & `invenio-communities-6.6.0/invenio_communities/members/services/schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/members/services/service.py` & `invenio-communities-6.6.0/invenio_communities/members/services/service.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/permissions.py` & `invenio-communities-6.6.0/invenio_communities/permissions.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     CommunityCurators,
     CommunityManagers,
     CommunityManagersForRole,
     CommunityMembers,
     CommunityOwners,
     CommunitySelfMember,
     GroupsEnabled,
+    IfConfig,
     IfPolicyClosed,
     IfRestricted,
 )
 
 
 # Permission Policy
 class CommunityPermissionPolicy(BasePermissionPolicy):
@@ -46,14 +47,22 @@
         SystemProcess(),
     ]
 
     can_update = [CommunityOwners(), SystemProcess()]
 
     can_delete = [CommunityOwners(), SystemProcess()]
 
+    can_manage_access = [
+        IfConfig("COMMUNITIES_ALLOW_RESTRICTED", then_=can_update, else_=[]),
+    ]
+
+    can_create_restricted = [
+        IfConfig("COMMUNITIES_ALLOW_RESTRICTED", then_=can_create, else_=[]),
+    ]
+
     can_search = [AnyUser(), SystemProcess()]
 
     can_search_user_communities = [AuthenticatedUser(), SystemProcess()]
 
     can_search_invites = [CommunityManagers(), SystemProcess()]
 
     can_search_requests = [CommunityManagers(), CommunityCurators(), SystemProcess()]
```

### Comparing `invenio-communities-6.5.0/invenio_communities/proxies.py` & `invenio-communities-6.6.0/invenio_communities/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/records/records/models.py` & `invenio-communities-6.6.0/invenio_communities/records/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/records/records/systemfields/communities/context.py` & `invenio-communities-6.6.0/invenio_communities/records/records/systemfields/communities/context.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/records/records/systemfields/communities/field.py` & `invenio-communities-6.6.0/invenio_communities/records/records/systemfields/communities/field.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/records/records/systemfields/communities/manager.py` & `invenio-communities-6.6.0/invenio_communities/records/records/systemfields/communities/manager.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/roles.py` & `invenio-communities-6.6.0/invenio_communities/roles.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/searchapp.py` & `invenio-communities-6.6.0/invenio_communities/searchapp.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/about/index.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/about/index.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/index.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/index.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/header.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/header.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/custom_fields.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/custom_fields.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/invitations.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/invitations.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/members.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/members.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/index.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/index.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html`

 * *Files 23% similar despite different names*

```diff
@@ -17,85 +17,128 @@
 00000100: 636f 6d6d 756e 6974 6965 732f 6465 7461  communities/deta
 00000110: 696c 732f 6261 7365 2e68 746d 6c22 2025  ils/base.html" %
 00000120: 7d0a 0a7b 252d 2073 6574 2074 6974 6c65  }..{%- set title
 00000130: 203d 2063 6f6d 6d75 6e69 7479 2e6d 6574   = community.met
 00000140: 6164 6174 612e 7469 746c 6520 2b20 5f28  adata.title + _(
 00000150: 2220 7365 7474 696e 6773 2229 202d 257d  " settings") -%}
 00000160: 0a0a 7b25 2d20 626c 6f63 6b20 7061 6765  ..{%- block page
-00000170: 5f62 6f64 7920 257d 0a7b 7b20 7375 7065  _body %}.{{ supe
-00000180: 7228 2920 7d7d 0a3c 6469 7620 2063 6c61  r() }}.<div  cla
-00000190: 7373 3d22 7569 2063 6f6e 7461 696e 6572  ss="ui container
-000001a0: 2067 7269 6420 636f 6d6d 756e 6974 6965   grid communitie
-000001b0: 732d 7365 7474 696e 6773 2072 656c 2d6d  s-settings rel-m
-000001c0: 742d 3222 3e0a 2020 7b25 2d20 626c 6f63  t-2">.  {%- bloc
-000001d0: 6b20 7365 7474 696e 6773 5f6d 656e 7520  k settings_menu 
-000001e0: 257d 0a20 2020 207b 252d 2073 6574 206d  %}.    {%- set m
-000001f0: 656e 755f 6974 656d 7320 3d20 7b0a 2020  enu_items = {.  
-00000200: 2020 2020 2770 726f 6669 6c65 273a 2028      'profile': (
-00000210: 5f28 2750 726f 6669 6c65 2729 2c20 7572  _('Profile'), ur
-00000220: 6c5f 666f 7228 2769 6e76 656e 696f 5f63  l_for('invenio_c
-00000230: 6f6d 6d75 6e69 7469 6573 2e63 6f6d 6d75  ommunities.commu
-00000240: 6e69 7469 6573 5f73 6574 7469 6e67 7327  nities_settings'
-00000250: 2c20 7069 645f 7661 6c75 653d 636f 6d6d  , pid_value=comm
-00000260: 756e 6974 792e 736c 7567 292c 2029 2c0a  unity.slug), ),.
-00000270: 2020 2020 2020 2770 7269 7669 6c65 6765        'privilege
-00000280: 7327 3a20 285f 2827 5072 6976 696c 6567  s': (_('Privileg
-00000290: 6573 2729 2c20 7572 6c5f 666f 7228 2769  es'), url_for('i
-000002a0: 6e76 656e 696f 5f63 6f6d 6d75 6e69 7469  nvenio_communiti
-000002b0: 6573 2e63 6f6d 6d75 6e69 7469 6573 5f73  es.communities_s
-000002c0: 6574 7469 6e67 735f 7072 6976 696c 6567  ettings_privileg
-000002d0: 6573 272c 2070 6964 5f76 616c 7565 3d63  es', pid_value=c
-000002e0: 6f6d 6d75 6e69 7479 2e73 6c75 6729 292c  ommunity.slug)),
-000002f0: 0a20 2020 2020 2027 6375 7261 7469 6f6e  .      'curation
-00000300: 5f70 6f6c 6963 7927 3a20 285f 2827 4375  _policy': (_('Cu
-00000310: 7261 7469 6f6e 2070 6f6c 6963 7927 292c  ration policy'),
-00000320: 2075 726c 5f66 6f72 2827 696e 7665 6e69   url_for('inveni
-00000330: 6f5f 636f 6d6d 756e 6974 6965 732e 636f  o_communities.co
-00000340: 6d6d 756e 6974 6965 735f 7365 7474 696e  mmunities_settin
-00000350: 6773 5f63 7572 6174 696f 6e5f 706f 6c69  gs_curation_poli
-00000360: 6379 272c 2070 6964 5f76 616c 7565 3d63  cy', pid_value=c
-00000370: 6f6d 6d75 6e69 7479 2e73 6c75 6729 292c  ommunity.slug)),
-00000380: 0a20 2020 2020 2027 7061 6765 7327 3a20  .      'pages': 
-00000390: 285f 2827 5061 6765 7327 292c 2075 726c  (_('Pages'), url
-000003a0: 5f66 6f72 2827 696e 7665 6e69 6f5f 636f  _for('invenio_co
-000003b0: 6d6d 756e 6974 6965 732e 636f 6d6d 756e  mmunities.commun
-000003c0: 6974 6965 735f 7365 7474 696e 6773 5f70  ities_settings_p
-000003d0: 6167 6573 272c 2070 6964 5f76 616c 7565  ages', pid_value
-000003e0: 3d63 6f6d 6d75 6e69 7479 2e73 6c75 6729  =community.slug)
-000003f0: 292c 0a20 2020 207d 2025 7d0a 2020 2020  ),.    } %}.    
-00000400: 3c64 6976 2063 6c61 7373 3d22 7369 7874  <div class="sixt
-00000410: 6565 6e20 7769 6465 206d 6f62 696c 6520  een wide mobile 
-00000420: 7369 7874 6565 6e20 7769 6465 2074 6162  sixteen wide tab
-00000430: 6c65 7420 7468 7265 6520 7769 6465 2063  let three wide c
-00000440: 6f6d 7075 7465 7220 636f 6c75 6d6e 223e  omputer column">
-00000450: 0a20 2020 2020 203c 6469 7620 636c 6173  .      <div clas
-00000460: 733d 2275 6920 7665 7274 6963 616c 2068  s="ui vertical h
-00000470: 6f72 697a 6f6e 7461 6c20 6d6f 6269 6c65  orizontal mobile
-00000480: 2074 6162 6c65 7420 6d65 6e75 223e 0a20   tablet menu">. 
-00000490: 2020 2020 2020 207b 2520 666f 7220 6d65         {% for me
-000004a0: 6e75 5f6b 6579 2c20 286d 656e 755f 6974  nu_key, (menu_it
-000004b0: 656d 2c20 6d65 6e75 5f6c 696e 6b2c 2029  em, menu_link, )
-000004c0: 2069 6e20 6d65 6e75 5f69 7465 6d73 2e69   in menu_items.i
-000004d0: 7465 6d73 2829 2025 7d0a 2020 2020 2020  tems() %}.      
-000004e0: 2020 2020 3c61 2068 7265 663d 227b 7b20      <a href="{{ 
-000004f0: 6d65 6e75 5f6c 696e 6b20 7d7d 2220 636c  menu_link }}" cl
-00000500: 6173 733d 227b 7b20 2762 7261 6e64 2069  ass="{{ 'brand i
-00000510: 7465 6d20 6163 7469 7665 2720 6966 2061  tem active' if a
-00000520: 6374 6976 655f 7365 7474 696e 6773 5f6d  ctive_settings_m
-00000530: 656e 755f 6974 656d 2061 6e64 206d 656e  enu_item and men
-00000540: 755f 6b65 7920 3d3d 2061 6374 6976 655f  u_key == active_
-00000550: 7365 7474 696e 6773 5f6d 656e 755f 6974  settings_menu_it
-00000560: 656d 207d 7d20 7b7b 2027 6469 7361 626c  em }} {{ 'disabl
-00000570: 6564 2720 6966 206e 6f74 206d 656e 755f  ed' if not menu_
-00000580: 6c69 6e6b 207d 7d20 6974 656d 223e 7b7b  link }} item">{{
-00000590: 206d 656e 755f 6974 656d 207d 7d3c 2f61   menu_item }}</a
-000005a0: 3e0a 2020 2020 2020 2020 7b25 2065 6e64  >.        {% end
-000005b0: 666f 7220 257d 0a20 2020 2020 203c 2f64  for %}.      </d
-000005c0: 6976 3e0a 2020 2020 3c2f 6469 763e 0a0a  iv>.    </div>..
-000005d0: 2020 7b25 2d20 656e 6462 6c6f 636b 2073    {%- endblock s
-000005e0: 6574 7469 6e67 735f 6d65 6e75 2025 7d0a  ettings_menu %}.
-000005f0: 2020 7b25 2d20 626c 6f63 6b20 7365 7474    {%- block sett
-00000600: 696e 6773 5f62 6f64 7920 257d 0a20 207b  ings_body %}.  {
-00000610: 252d 2065 6e64 626c 6f63 6b20 7365 7474  %- endblock sett
-00000620: 696e 6773 5f62 6f64 7920 257d 0a3c 2f64  ings_body %}.</d
-00000630: 6976 3e0a 7b25 2d20 656e 6462 6c6f 636b  iv>.{%- endblock
-00000640: 2070 6167 655f 626f 6479 2025 7d0a        page_body %}.
+00000170: 5f62 6f64 7920 257d 0a20 207b 7b20 7375  _body %}.  {{ su
+00000180: 7065 7228 2920 7d7d 0a20 203c 6469 7620  per() }}.  <div 
+00000190: 636c 6173 733d 2275 6920 636f 6e74 6169  class="ui contai
+000001a0: 6e65 7220 6772 6964 2063 6f6d 6d75 6e69  ner grid communi
+000001b0: 7469 6573 2d73 6574 7469 6e67 7320 7265  ties-settings re
+000001c0: 6c2d 6d74 2d32 223e 0a0a 2020 2020 7b25  l-mt-2">..    {%
+000001d0: 2d20 626c 6f63 6b20 7365 7474 696e 6773  - block settings
+000001e0: 5f6d 656e 7520 257d 0a20 2020 2020 207b  _menu %}.      {
+000001f0: 252d 2073 6574 206d 656e 755f 6974 656d  %- set menu_item
+00000200: 7320 3d20 7b0a 2020 2020 2020 2020 2770  s = {.        'p
+00000210: 726f 6669 6c65 273a 2028 5f28 2750 726f  rofile': (_('Pro
+00000220: 6669 6c65 2729 2c20 7572 6c5f 666f 7228  file'), url_for(
+00000230: 2769 6e76 656e 696f 5f63 6f6d 6d75 6e69  'invenio_communi
+00000240: 7469 6573 2e63 6f6d 6d75 6e69 7469 6573  ties.communities
+00000250: 5f73 6574 7469 6e67 7327 2c20 7069 645f  _settings', pid_
+00000260: 7661 6c75 653d 636f 6d6d 756e 6974 792e  value=community.
+00000270: 736c 7567 2929 2c0a 2020 2020 2020 2020  slug)),.        
+00000280: 2770 7269 7669 6c65 6765 7327 3a20 285f  'privileges': (_
+00000290: 2827 5072 6976 696c 6567 6573 2729 2c20  ('Privileges'), 
+000002a0: 7572 6c5f 666f 7228 2769 6e76 656e 696f  url_for('invenio
+000002b0: 5f63 6f6d 6d75 6e69 7469 6573 2e63 6f6d  _communities.com
+000002c0: 6d75 6e69 7469 6573 5f73 6574 7469 6e67  munities_setting
+000002d0: 735f 7072 6976 696c 6567 6573 272c 2070  s_privileges', p
+000002e0: 6964 5f76 616c 7565 3d63 6f6d 6d75 6e69  id_value=communi
+000002f0: 7479 2e73 6c75 6729 292c 0a20 2020 2020  ty.slug)),.     
+00000300: 2020 2027 6375 7261 7469 6f6e 5f70 6f6c     'curation_pol
+00000310: 6963 7927 3a20 285f 2827 4375 7261 7469  icy': (_('Curati
+00000320: 6f6e 2070 6f6c 6963 7927 292c 2075 726c  on policy'), url
+00000330: 5f66 6f72 2827 696e 7665 6e69 6f5f 636f  _for('invenio_co
+00000340: 6d6d 756e 6974 6965 732e 636f 6d6d 756e  mmunities.commun
+00000350: 6974 6965 735f 7365 7474 696e 6773 5f63  ities_settings_c
+00000360: 7572 6174 696f 6e5f 706f 6c69 6379 272c  uration_policy',
+00000370: 2070 6964 5f76 616c 7565 3d63 6f6d 6d75   pid_value=commu
+00000380: 6e69 7479 2e73 6c75 6729 292c 0a20 2020  nity.slug)),.   
+00000390: 2020 2020 2027 7061 6765 7327 3a20 285f       'pages': (_
+000003a0: 2827 5061 6765 7327 292c 2075 726c 5f66  ('Pages'), url_f
+000003b0: 6f72 2827 696e 7665 6e69 6f5f 636f 6d6d  or('invenio_comm
+000003c0: 756e 6974 6965 732e 636f 6d6d 756e 6974  unities.communit
+000003d0: 6965 735f 7365 7474 696e 6773 5f70 6167  ies_settings_pag
+000003e0: 6573 272c 2070 6964 5f76 616c 7565 3d63  es', pid_value=c
+000003f0: 6f6d 6d75 6e69 7479 2e73 6c75 6729 292c  ommunity.slug)),
+00000400: 0a20 2020 2020 207d 2025 7d0a 2020 2020  .      } %}.    
+00000410: 2020 3c64 6976 2063 6c61 7373 3d22 7369    <div class="si
+00000420: 7874 6565 6e20 7769 6465 206d 6f62 696c  xteen wide mobil
+00000430: 6520 7369 7874 6565 6e20 7769 6465 2074  e sixteen wide t
+00000440: 6162 6c65 7420 7468 7265 6520 7769 6465  ablet three wide
+00000450: 2063 6f6d 7075 7465 7220 636f 6c75 6d6e   computer column
+00000460: 223e 0a20 2020 2020 2020 203c 6469 7620  ">.        <div 
+00000470: 726f 6c65 3d22 7461 626c 6973 7422 2063  role="tablist" c
+00000480: 6c61 7373 3d22 7569 2076 6572 7469 6361  lass="ui vertica
+00000490: 6c20 686f 7269 7a6f 6e74 616c 206d 6f62  l horizontal mob
+000004a0: 696c 6520 7461 626c 6574 206d 656e 7522  ile tablet menu"
+000004b0: 3e0a 2020 2020 2020 2020 2020 7b25 2066  >.          {% f
+000004c0: 6f72 206d 656e 755f 6b65 792c 2028 6d65  or menu_key, (me
+000004d0: 6e75 5f69 7465 6d2c 206d 656e 755f 6c69  nu_item, menu_li
+000004e0: 6e6b 2920 696e 206d 656e 755f 6974 656d  nk) in menu_item
+000004f0: 732e 6974 656d 7328 2920 257d 0a20 2020  s.items() %}.   
+00000500: 2020 2020 2020 2020 207b 2520 6966 206e           {% if n
+00000510: 6f74 2028 6d65 6e75 5f6b 6579 203d 3d20  ot (menu_key == 
+00000520: 2770 7269 7669 6c65 6765 7327 2061 6e64  'privileges' and
+00000530: 206e 6f74 2070 6572 6d69 7373 696f 6e73   not permissions
+00000540: 2e63 616e 5f6d 616e 6167 655f 6163 6365  .can_manage_acce
+00000550: 7373 2920 257d 0a20 2020 2020 2020 2020  ss) %}.         
+00000560: 2020 2020 203c 610a 2020 2020 2020 2020       <a.        
+00000570: 2020 2020 2020 2020 726f 6c65 3d22 7461          role="ta
+00000580: 6222 0a20 2020 2020 2020 2020 2020 2020  b".             
+00000590: 2020 2069 643d 227b 7b20 6d65 6e75 5f6b     id="{{ menu_k
+000005a0: 6579 207d 7d22 0a20 2020 2020 2020 2020  ey }}".         
+000005b0: 2020 2020 2020 2061 7269 612d 7365 6c65         aria-sele
+000005c0: 6374 6564 3d22 7b7b 2061 6374 6976 655f  cted="{{ active_
+000005d0: 7365 7474 696e 6773 5f6d 656e 755f 6974  settings_menu_it
+000005e0: 656d 2061 6e64 206d 656e 755f 6b65 7920  em and menu_key 
+000005f0: 3d3d 2061 6374 6976 655f 7365 7474 696e  == active_settin
+00000600: 6773 5f6d 656e 755f 6974 656d 207d 7d22  gs_menu_item }}"
+00000610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000620: 2068 7265 663d 227b 7b20 6d65 6e75 5f6c   href="{{ menu_l
+00000630: 696e 6b20 7d7d 220a 2020 2020 2020 2020  ink }}".        
+00000640: 2020 2020 2020 2020 636c 6173 733d 227b          class="{
+00000650: 7b20 2762 7261 6e64 2069 7465 6d20 6163  { 'brand item ac
+00000660: 7469 7665 2720 6966 2061 6374 6976 655f  tive' if active_
+00000670: 7365 7474 696e 6773 5f6d 656e 755f 6974  settings_menu_it
+00000680: 656d 2061 6e64 206d 656e 755f 6b65 7920  em and menu_key 
+00000690: 3d3d 2061 6374 6976 655f 7365 7474 696e  == active_settin
+000006a0: 6773 5f6d 656e 755f 6974 656d 207d 7d20  gs_menu_item }} 
+000006b0: 7b7b 2027 6469 7361 626c 6564 2720 6966  {{ 'disabled' if
+000006c0: 206e 6f74 206d 656e 755f 6c69 6e6b 207d   not menu_link }
+000006d0: 7d20 6974 656d 220a 2020 2020 2020 2020  } item".        
+000006e0: 2020 2020 2020 2020 3e7b 7b20 6d65 6e75          >{{ menu
+000006f0: 5f69 7465 6d20 7d7d 3c2f 610a 2020 2020  _item }}</a.    
+00000700: 2020 2020 2020 2020 2020 3e0a 2020 2020            >.    
+00000710: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+00000720: 2025 7d0a 2020 2020 2020 2020 2020 7b25   %}.          {%
+00000730: 2065 6e64 666f 7220 257d 0a20 2020 2020   endfor %}.     
+00000740: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00000750: 3c2f 6469 763e 0a20 2020 207b 252d 2065  </div>.    {%- e
+00000760: 6e64 626c 6f63 6b20 7365 7474 696e 6773  ndblock settings
+00000770: 5f6d 656e 7520 257d 0a0a 2020 2020 3c64  _menu %}..    <d
+00000780: 6976 0a20 2020 2020 2072 6f6c 653d 2274  iv.      role="t
+00000790: 6162 7061 6e65 6c22 0a20 2020 2020 2069  abpanel".      i
+000007a0: 643d 227b 7b20 6163 7469 7665 5f73 6574  d="{{ active_set
+000007b0: 7469 6e67 735f 6d65 6e75 5f69 7465 6d20  tings_menu_item 
+000007c0: 7d7d 2d70 616e 656c 220a 2020 2020 2020  }}-panel".      
+000007d0: 6172 6961 2d65 7870 616e 6465 643d 2274  aria-expanded="t
+000007e0: 7275 6522 0a20 2020 2020 2068 6964 6465  rue".      hidde
+000007f0: 6e3d 2266 616c 7365 220a 2020 2020 2020  n="false".      
+00000800: 6172 6961 2d6c 6162 656c 6c65 6462 793d  aria-labelledby=
+00000810: 227b 7b20 6163 7469 7665 5f73 6574 7469  "{{ active_setti
+00000820: 6e67 735f 6d65 6e75 5f69 7465 6d20 7d7d  ngs_menu_item }}
+00000830: 220a 2020 2020 2020 636c 6173 733d 2273  ".      class="s
+00000840: 6978 7465 656e 2077 6964 6520 6d6f 6269  ixteen wide mobi
+00000850: 6c65 2073 6978 7465 656e 2077 6964 6520  le sixteen wide 
+00000860: 7461 626c 6574 2074 6869 7274 6565 6e20  tablet thirteen 
+00000870: 7769 6465 2063 6f6d 7075 7465 7220 636f  wide computer co
+00000880: 6c75 6d6e 220a 2020 2020 3e0a 2020 2020  lumn".    >.    
+00000890: 2020 7b25 2d20 626c 6f63 6b20 7365 7474    {%- block sett
+000008a0: 696e 6773 5f62 6f64 7920 257d 0a20 2020  ings_body %}.   
+000008b0: 2020 207b 252d 2065 6e64 626c 6f63 6b20     {%- endblock 
+000008c0: 7365 7474 696e 6773 5f62 6f64 7920 257d  settings_body %}
+000008d0: 0a20 2020 203c 2f64 6976 3e0a 2020 3c2f  .    </div>.  </
+000008e0: 6469 763e 0a7b 252d 2065 6e64 626c 6f63  div>.{%- endbloc
+000008f0: 6b20 7061 6765 5f62 6f64 7920 257d 0a    k page_body %}.
```

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/curation_policy.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/curation_policy.html`

 * *Files 14% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 {{ webpack['invenio-communities-curation-policy.js'] }}
 {%- endblock javascript %}
 
 {% set active_settings_menu_item = 'curation_policy' %}
 {% set active_community_header_menu_item = 'settings' %}
 
 {%- block settings_body %}
-<div class="sixteen wide mobile sixteen wide tablet thirteen wide computer column">
   <div
     id="app"
     data-community='{{ community | tojson }}'
     data-form-config='{{ form_config | tojson }}'
   >
   </div>
-</div>
 {%- endblock settings_body %}
```

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/pages.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/pages.html`

 * *Files 13% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 {{ webpack['invenio-communities-settings-pages.js'] }}
 {%- endblock javascript %}
 
 {% set active_settings_menu_item = 'pages' %}
 {% set active_community_header_menu_item = 'settings' %}
 
 {%- block settings_body %}
-<div class="sixteen wide mobile sixteen wide tablet thirteen wide computer column">
   <div
     id="community-settings-pages"
     data-community='{{ community | tojson }}'
     data-form-config='{{ form_config | tojson }}'
   >
   </div>
-</div>
 {%- endblock settings_body %}
```

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/privileges.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/privileges.html`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,13 @@
 {{ webpack['invenio-communities-privileges.js'] }}
 {%- endblock javascript %}
 
 {% set active_settings_menu_item = 'privileges' %}
 {% set active_community_header_menu_item = 'settings' %}
 
 {%- block settings_body %}
-<div class="sixteen wide mobile sixteen wide tablet thirteen wide computer column">
   <div
     id="app"
     data-form-config='{{ form_config | tojson }}'
     data-community='{{ community | tojson}}'>
   </div>
-</div>
 {%- endblock settings_body %}
```

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/profile.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/profile.html`

 * *Files 15% similar despite different names*

```diff
@@ -14,19 +14,17 @@
 {{ webpack['invenio-communities-profile.js'] }}
 {%- endblock javascript %}
 
 {% set active_settings_menu_item = 'profile' %}
 {% set active_community_header_menu_item = 'settings' %}
 
 {%- block settings_body %}
-<div class="sixteen wide mobile sixteen wide tablet thirteen wide computer column">
   <div
     id="app"
     data-community='{{ community | tojson}}'
     data-has-logo='{{ has_logo | tojson }}'
     data-types='{{ types | tojson }}'
     data-logo-max-size='{{ logo_quota | tojson }}'
     data-custom-fields='{{ custom_fields | tojson }}'
   >
   </div>
-</div>
 {%- endblock settings_body %}
```

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/featured_communities.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/featured_communities.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/new.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/request.html`

 * *Files 15% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 
   Invenio is free software; you can redistribute it and/or modify it
   under the terms of the MIT License; see LICENSE file for more details.
 #}
 
 {% extends "invenio_communities/base.html" %}
 
-{%- set title = _("New community") -%}
-
 {%- block javascript %}
-{{ super() }}
-{{ webpack['invenio-communities-new.js'] }}
+  {{ super() }}
+  {{ webpack['invenio-communities-request.js'] }}
 {%- endblock javascript %}
 
 
 {%- block page_body %}
+{%- set form_config = {"community": community, "membership": membership, "token": token} %}
+
 <div
-    id="app"
-    data-form-config='{{ form_config | tojson }}'
-    data-custom-fields='{{ custom_fields | tojson }}'
-  >
+  id="app"
+  data-form-config='{{ form_config | tojson }}'>
 </div>
+
 {%- endblock page_body %}
+
+
```

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/search.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/search.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/templates/semantic-ui/invenio_communities/tombstone.html` & `invenio-communities-6.6.0/invenio_communities/templates/semantic-ui/invenio_communities/tombstone.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/af/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/af/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/ar/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/ar/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/bg/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/bg/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/ca/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/ca/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/cs/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/cs/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/da/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/da/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/de/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/de/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/el/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/el/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/en/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/es/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/es/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/et/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/et/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/fa/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/fa/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/fr/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/fr/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/gl/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/gl/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/hr/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/hr/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/hu/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/hu/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/it/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/it/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/ja/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/ja/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/ka/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/ka/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/lt/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/lt/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/messages.pot` & `invenio-communities-6.6.0/invenio_communities/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/no/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/no/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/pl/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/pl/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/pt/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/pt/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/ro/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/ro/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/ru/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/ru/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/rw/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/rw/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/sk/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/sk/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/sv/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/sv/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/tr/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/tr/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/uk/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/uk/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-communities-6.6.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-communities-6.6.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/utils.py` & `invenio-communities-6.6.0/invenio_communities/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/views/__init__.py` & `invenio-communities-6.6.0/invenio_communities/views/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/views/api.py` & `invenio-communities-6.6.0/invenio_communities/views/api.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/views/communities.py` & `invenio-communities-6.6.0/invenio_communities/views/communities.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,31 +146,43 @@
 
 @login_required
 def communities_new():
     """Communities creation page."""
     can_create = current_communities.service.check_permission(g.identity, "create")
     if not can_create:
         raise PermissionDeniedError()
+
+    can_create_restricted = current_communities.service.check_permission(
+        g.identity, "create_restricted"
+    )
+
     return render_template(
         "invenio_communities/new.html",
         form_config=dict(
             access=dict(visibility=VISIBILITY_FIELDS),
             SITE_UI_URL=current_app.config["SITE_UI_URL"],
         ),
         custom_fields=load_custom_fields(
             dump_only_required=True,
         ),
+        can_create_restricted=can_create_restricted,
     )
 
 
 @pass_community(serialize=True)
 def communities_settings(pid_value, community, community_ui):
     """Community settings/profile page."""
     permissions = community.has_permissions_to(
-        ["update", "read", "search_requests", "search_invites"]
+        [
+            "update",
+            "read",
+            "search_requests",
+            "search_invites",
+            "manage_access",
+        ]
     )
     if not permissions["can_update"]:
         raise PermissionDeniedError()
 
     _types = vocabulary_service.read_all(
         g.identity,
         fields=["id", "title"],
@@ -220,17 +232,24 @@
     )
 
 
 @pass_community(serialize=True)
 def communities_settings_privileges(pid_value, community, community_ui):
     """Community settings/privileges page."""
     permissions = community.has_permissions_to(
-        ["update", "read", "search_requests", "search_invites"]
+        [
+            "update",
+            "read",
+            "search_requests",
+            "search_invites",
+            "manage_access",
+        ]
     )
-    if not permissions["can_update"]:
+
+    if not permissions["can_manage_access"]:
         raise PermissionDeniedError()
 
     return render_template(
         "invenio_communities/details/settings/privileges.html",
         community=community_ui,
         form_config=dict(
             access=dict(visibility=VISIBILITY_FIELDS),
@@ -238,15 +257,18 @@
         permissions=permissions,
     )
 
 
 @pass_community(serialize=True)
 def communities_settings_curation_policy(pid_value, community, community_ui):
     """Community settings/curation-policy page."""
-    permissions = community.has_permissions_to(["update", "read", "search_requests"])
+    permissions = community.has_permissions_to(
+        ["update", "read", "search_requests", "manage_access"]
+    )
+
     if not permissions["can_update"]:
         raise PermissionDeniedError()
 
     return render_template(
         "invenio_communities/details/settings/curation_policy.html",
         community=community_ui,
         permissions=permissions,
@@ -256,15 +278,21 @@
     )
 
 
 @pass_community(serialize=True)
 def communities_settings_pages(pid_value, community, community_ui):
     """Community settings/curation-policy page."""
     permissions = community.has_permissions_to(
-        ["update", "read", "search_requests", "search_invites"]
+        [
+            "update",
+            "read",
+            "search_requests",
+            "search_invites",
+            "manage_access",
+        ]
     )
     if not permissions["can_update"]:
         raise PermissionDeniedError()
 
     return render_template(
         "invenio_communities/details/settings/pages.html",
         community=community_ui,
```

### Comparing `invenio-communities-6.5.0/invenio_communities/views/decorators.py` & `invenio-communities-6.6.0/invenio_communities/views/decorators.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities/views/ui.py` & `invenio-communities-6.6.0/invenio_communities/views/ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     """Handle permission denier error on record views."""
     if not current_user.is_authenticated:
         # trigger the flask-login unauthorized handler
         return current_app.login_manager.unauthorized()
     return render_template(current_app.config["THEME_403_TEMPLATE"]), 403
 
 
-def _can_create_comunity():
+def _can_create_community():
     """Function used to check if a user has permissions to create a community."""
     can_create = current_communities.service.check_permission(g.identity, "create")
     return can_create
 
 
 #
 # Registration
@@ -144,15 +144,15 @@
             "Communities",
             order=1,
         )
         current_menu.submenu("plus.community").register(
             "invenio_communities.communities_new",
             "New community",
             order=3,
-            visible_when=_can_create_comunity,
+            visible_when=_can_create_community,
         )
 
         communities = current_menu.submenu("communities")
 
         communities.submenu("requests").register(
             "invenio_communities.communities_requests",
             text=_("Requests"),
```

### Comparing `invenio-communities-6.5.0/invenio_communities/webpack.py` & `invenio-communities-6.6.0/invenio_communities/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities.egg-info/PKG-INFO` & `invenio-communities-6.6.0/invenio_communities.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-communities
-Version: 6.5.0
+Version: 6.6.0
 Summary: InvenioRDM module for the communities feature.
 Home-page: https://github.com/inveniosoftware/invenio-communities
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -45,14 +45,22 @@
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         
         Changes
         =======
         
+        Version 6.6.0 (released 2023-05-26)
+        -----------------------------------
+        
+        - configure number of items in communities carousel
+        - add placeholder in communities carousel
+        - introduce a configuration to disallow the creation of a restricted community
+        - fix a11y for tabs and modals in communities settings
+        
         Version 6.5.0 (released 2023-05-05)
         -----------------------------------
         
         - update mappings of members and invitations
         - add configurable community permission policy
         
         Version 6.4.0 (released 2023-04-25)
```

### Comparing `invenio-communities-6.5.0/invenio_communities.egg-info/SOURCES.txt` & `invenio-communities-6.6.0/invenio_communities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/invenio_communities.egg-info/entry_points.txt` & `invenio-communities-6.6.0/invenio_communities.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/run-js-linter.sh` & `invenio-communities-6.6.0/run-js-linter.sh`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/run-tests.sh` & `invenio-communities-6.6.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/setup.cfg` & `invenio-communities-6.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/communities/conftest.py` & `invenio-communities-6.6.0/tests/communities/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/communities/test_alembic.py` & `invenio-communities-6.6.0/tests/communities/test_alembic.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/communities/test_cli.py` & `invenio-communities-6.6.0/tests/communities/test_cli.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/communities/test_community_ui_serializer.py` & `invenio-communities-6.6.0/tests/communities/test_community_ui_serializer.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/communities/test_components.py` & `invenio-communities-6.6.0/tests/communities/test_components.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/communities/test_relations_organizations.py` & `invenio-communities-6.6.0/tests/communities/test_relations_organizations.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/communities/test_relations_types.py` & `invenio-communities-6.6.0/tests/communities/test_relations_types.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/communities/test_resources.py` & `invenio-communities-6.6.0/tests/communities/test_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -781,7 +781,134 @@
 
     # featured entry does not exist
     res = client.put(f"/communities/{c_id_}/featured/0", headers=headers, json={})
     assert res.status_code == 404
 
     res = client.delete(f"/communities/{c_id_}/featured/0", headers=headers)
     assert res.status_code == 404
+
+
+def test_simple_flow_restricted_community(
+    app,
+    client,
+    location,
+    minimal_restricted_community_1,
+    minimal_restricted_community_2,
+    headers,
+    owner,
+    db,
+):
+    """Test a simple REST API flow."""
+    client = owner.login(client)
+
+    # Create a community
+    res = client.post(
+        "/communities", headers=headers, json=minimal_restricted_community_1
+    )
+    Member.index.refresh()
+
+    assert res.status_code == 201
+    _assert_single_item_response(res)
+    created_community = res.json
+    id_ = created_community["id"]
+    slug = created_community["slug"]
+
+    # Read the community
+    res = client.get(f"/communities/{id_}", headers=headers)
+    assert res.status_code == 200
+    assert res.json["metadata"] == created_community["metadata"]
+
+    read_community = res.json
+    Community.index.refresh()
+
+    app.config["COMMUNITIES_ALLOW_RESTRICTED"] = False
+
+    # Create a new community, which should default to public
+    res = client.post(
+        "/communities", headers=headers, json=minimal_restricted_community_2
+    )
+    Member.index.refresh()
+
+    assert res.status_code == 403
+
+
+def test_permissions_modify_community_visibility(
+    app,
+    client,
+    location,
+    minimal_community,
+    headers,
+    owner,
+    db,
+):
+    """Test modifying community visibility."""
+
+    app.config["COMMUNITIES_ALLOW_RESTRICTED"] = False
+
+    client = owner.login(client)
+    # Create a public community
+    res = client.post("/communities", headers=headers, json=minimal_community)
+    Member.index.refresh()
+
+    assert res.status_code == 201
+    _assert_single_item_response(res)
+
+    created_community = res.json
+    id_ = created_community["id"]
+    slug = created_community["slug"]
+
+    # Read the community
+    res = client.get(f"/communities/{id_}", headers=headers)
+    assert res.status_code == 200
+    assert res.json["metadata"] == created_community["metadata"]
+
+    read_community = res.json
+    Community.index.refresh()
+
+    # try to change public community to restricted
+    data = copy.deepcopy(read_community)
+    data["metadata"]["title"] = "New title"
+    data["access"]["visibility"] = "restricted"
+    res = client.put(f"/communities/{id_}", headers=headers, json=data)
+    assert res.status_code == 403
+
+
+def test_permissions_modify_community_to_public(
+    app,
+    client,
+    location,
+    minimal_restricted_community_1,
+    headers,
+    owner,
+    db,
+):
+    """Test modifying community visibility."""
+    app.config["COMMUNITIES_ALLOW_RESTRICTED"] = True
+    client = owner.login(client)
+    # Create a public community
+    res = client.post(
+        "/communities", headers=headers, json=minimal_restricted_community_1
+    )
+    Member.index.refresh()
+
+    assert res.status_code == 201
+    _assert_single_item_response(res)
+
+    created_community = res.json
+    id_ = created_community["id"]
+    slug = created_community["slug"]
+
+    # Read the community
+    res = client.get(f"/communities/{id_}", headers=headers)
+    assert res.status_code == 200
+    assert res.json["metadata"] == created_community["metadata"]
+
+    read_community = res.json
+    Community.index.refresh()
+    app.config["COMMUNITIES_ALLOW_RESTRICTED"] = False
+
+    # try to change public community to restricted
+    data = copy.deepcopy(read_community)
+    data["metadata"]["title"] = "New title"
+    data["access"]["visibility"] = "public"
+    res = client.put(f"/communities/{id_}", headers=headers, json=data)
+    assert res.status_code == 403
```

### Comparing `invenio-communities-6.5.0/tests/communities/test_services.py` & `invenio-communities-6.6.0/tests/communities/test_services.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/communities/tests_views.py` & `invenio-communities-6.6.0/tests/communities/tests_views.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/conftest.py` & `invenio-communities-6.6.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -272,14 +272,44 @@
         "metadata": {
             "title": "My Community",
         },
     }
 
 
 @pytest.fixture(scope="module")
+def minimal_restricted_community_1():
+    """Minimal restricted community metadata."""
+    return {
+        "access": {
+            "visibility": "restricted",
+            "record_policy": "closed",
+        },
+        "slug": "community1",
+        "metadata": {
+            "title": "Community 1",
+        },
+    }
+
+
+@pytest.fixture(scope="module")
+def minimal_restricted_community_2():
+    """Minimal restricted community metadata."""
+    return {
+        "access": {
+            "visibility": "restricted",
+            "record_policy": "closed",
+        },
+        "slug": "community2",
+        "metadata": {
+            "title": "Community 2",
+        },
+    }
+
+
+@pytest.fixture(scope="module")
 def full_community():
     """Full community data as dict coming from the external world."""
     return {
         "access": {
             "visibility": "public",
             "member_policy": "open",
             "record_policy": "open",
```

### Comparing `invenio-communities-6.5.0/tests/members/conftest.py` & `invenio-communities-6.6.0/tests/members/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/members/test_members_components.py` & `invenio-communities-6.6.0/tests/members/test_members_components.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/members/test_members_no_groups.py` & `invenio-communities-6.6.0/tests/members/test_members_no_groups.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/members/test_members_resource.py` & `invenio-communities-6.6.0/tests/members/test_members_resource.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/members/test_members_services.py` & `invenio-communities-6.6.0/tests/members/test_members_services.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/records/conftest.py` & `invenio-communities-6.6.0/tests/records/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/records/mock_module/api.py` & `invenio-communities-6.6.0/tests/records/mock_module/api.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/records/mock_module/models.py` & `invenio-communities-6.6.0/tests/records/mock_module/models.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-6.5.0/tests/records/test_mockrecords_api.py` & `invenio-communities-6.6.0/tests/records/test_mockrecords_api.py`

 * *Files identical despite different names*

