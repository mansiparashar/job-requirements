# Job Requirements

## About
The goal of this project is to organize requirements found in current job listings for positions in the tech industry.:woman_technologist::man_technologist:

## Contribution
Submit PR for [Job Requirement data](/data/requirements.json), include as many of the following contributions as you'd like.  
Insert in alphabetical order :cool: this will help all contributors avoid duplicates.

:exclamation: Structure commit messages as one of the following:
 * `Add`**`requirement`**` to `**`category`** 
 * `Add`**`framework`**` to `**`requirement`**
 * `Add new category`**`category`**


![GitHub Hacktoberfest combined status (suggestion label override)](https://img.shields.io/github/hacktoberfest/2019/crystal-dawn/job-requirements?style=flat-square&suggestion_label=help%20wanted)
![GitHub issues](https://img.shields.io/github/issues-raw/crystal-dawn/job-requirements?style=flat-square)
 
### :star2: Contribute to Job Category
  * The initial categories are Data, Programming, Management, UI/UX
  
:warning: Categories should not be a job position  _e.g. Data Analyst, Frontend Developer, Project Manager, Graphic Designer_

  * Include at least an empty array for degrees, and minimum one example requirement     
```
"category": {                       // programming
  "degrees": [],
  "general job requirement": []     // JavaScript 
],
```
  * PR's for organizing data are accepted.

### :star2: Contribute to General Job Requirement
  * Job requirements are structured as arrays with nested objects for specific requirements - such as frameworks/libraries. 
  * Job rquirements do not need to include a specific framework/library, but should include an empty array if not.
```
"existing category": {...               // e.g. data analysis 
  "new requirement": []                 // e.g. databases
...}
```  
       
### :star2: Contribute to Specific Job Requirement
  * Nest frameworks/libraries, or otherwise applicable sub-requirements, under general requirement
  * Requirements are structured as name & url key/value pairs
    * URL's
       * Official documentation
       * Official user guide
       * Official certification page
``` 
"existing general requirement": [
  {
   "name": "new specific requirement",       // AngularJS
   "url": "docs for specific requirement"    // https://docs.angularjs.org/guide
  },      
]
```
  * The same job requirement may be listed under multiple categories.
```
  "data analysis": {...
    "databases": [
      {
        "name": "MongoDB",
        "url": "https://www.mongodb.com/datasheets"
      }
    ],
...},
 "programming": {...
    "databases": [
      {
        "name": "MongoDB",
        "url": "https://www.mongodb.com/datasheets"
      }
    ],
...},
```

## License
![GitHub](https://img.shields.io/github/license/crystal-dawn/job-requirements?style=flat-square)
