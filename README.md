# Elasticsearch Grails plugin - Sample App #

A sample app for the Elasticsearch Grails plugin. The plugin homepage is maintained by Noam Y. Tenne and hosted at https://github.com/noamt/elasticsearch-grails-plugin.

## Why? ##

If you're used to grails but have never used [Elasticsearch](http://www.elasticsearch.org/), chances are you'll be a bit lost after installing the plugin.
Elasticsearch is as powerful as it is complicated to understand for the newcomers.

This sample app aims to make it easier on users to get what the plugin actually enables in terms of mapping, indexing and searching via ES.

## How ##

In order to fully understand the relationship between the different cases implemented with this project, it is recommended to use it in the following way:

  * Experiment with the different available client modes by changing the options in `Config.groovy`

### Domains

The domains in this application try to use as extensiveley the mapping options provided by the plugin. To find a specific mapping, please refer to the following list:

**Domain class TODO**

  - [x] `parent` / `child` mapping (in `Musician` and `Song` domains).
  - [x] `geoPoint` mapping (in `Location` domain).
  - [ ] `multi_field` mapping.
  - [ ] `converter` mapping.
  - [ ] `excludeFromAll` mapping.
  - [ ] `index` mapping.
  - [ ] `analyzer` mapping.

In order to understand the impact of each mapping option, it is strongly recommended that you check the `JSON` results after launching the app using curl. Your command should look like the following:

````
  curl -XGET localhost:9200/org.elasticsearch.plugin.sample/_mapping?pretty
````




## License ##

````
/*
 * Copyright 2013-14 the original author or authors.
 *
 * Licensed under the Apache License, Version 2.0 (the "License");
 * you may not use this file except in compliance with the License.
 * You may obtain a copy of the License at
 *
 *      http://www.apache.org/licenses/LICENSE-2.0
 *
 * Unless required by applicable law or agreed to in writing, software
 * distributed under the License is distributed on an "AS IS" BASIS,
 * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 * See the License for the specific language governing permissions and
 * limitations under the License.
 */
````

## Here, have a donkey ##

````
         __
 __   (__`\
(__`\   \\`\
 `\\`\   \\ \
   `\\`\  \\ \
     `\\`\#\\ \#
       \_ ##\_ |##
       (___)(___)##
        (0)  (0)`\##
         |~   ~ , \##
         |      |  \##
         |     /\   \##         __..---'''''-.._.._
         |     | \   `\##  _.--'                _  `.
         Y     |  \    `##'                     \`\  \
        /      |   \                             | `\ \
       /_...___|    \                            |   `\\
      /        `.    |                          /      ##
     |          |    |                         /      ####
     |          |    |                        /       ####
     | () ()    |     \     |          |  _.-'         ##
     `.        .'      `._. |______..| |-'|
       `------'           | | | |    | || |
                          | | | |    | || |
                          | | | |    | || |
                          | | | |    | || |     Joan Stark
                    _____ | | | |____| || |
               jgs /     `` |-`/     ` |` |
                   \________\__\_______\__\
                    """""""""   """""""'"""
````