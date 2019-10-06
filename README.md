# Job Requirements

## About
The goal of this project is to organize requirements found in current job listings for positions in the tech industry.:woman_technologist::man_technologist:

## Contribution


:information_source: [Job Requirement data](/data/requirements.json) is organized by category (Data Analysis, Programming, etc.) then requirements (SQL, JavaScript, etc.) as it fits into each category.

:exclamation: Structure commit messages as one of the following:
 * `Add`**`requirement`**` to `**`category`** 
 * `Add`**`framework`**` to `**`requirement`**
 * `Add new category`**`category`**`
 
:warning: Insert in alphabetical order :cool: this will help all contributors avoid duplicates


![GitHub Hacktoberfest combined status (suggestion label override)](https://img.shields.io/github/hacktoberfest/2019/crystal-dawn/job-requirements?style=flat-square&suggestion_label=help%20wanted)
![GitHub issues](https://img.shields.io/github/issues-raw/crystal-dawn/job-requirements?style=flat-square)
 
### :star2: Contribute to Job Requirement Category
:warning: Categories should not be a job position
  * Include at least an empty array for degrees, and minimum one example requirement 
```
"high-level category": {
  "degrees": [],
  "requirement": "url"
},
```

  * As new job categories are added, PRs to reorganize existing requirements may be submitted.

### :star2:Contribute to Job Requirement
  
  * Requirements are structured as name/url key/value pairs
     * URL's
       * Official documentation
       * Official user guide
       * Official certification page
```
"project management": {...,
    "Microsoft Project": "https://docs.microsoft.com/en-us/projectonline/project-online",
},
```
  
  * Nest frameworks under higher-level requirement
```    
"JavaScript": {
    "AngularJS": "https://docs.angularjs.org/guide",
    "React": "https://reactjs.org/docs/getting-started.html"
}, 
```
  
  * Ensure requirement is properly cased (_PR's for corrections will be accepted_)
```
// bad
javascript
Javascript

// good
JavaScript
```

  * The same job requirement may be listed under multiple categories.
```
"data analysis": {...,
    "databases": { "MongoDB":  "https://www.mongodb.com/datasheets" }
},
"programming": {...,
    "databases": { "MongoDB":  "https://www.mongodb.com/datasheets" }
},
```

## License
![GitHub](https://img.shields.io/github/license/crystal-dawn/job-requirements?style=flat-square)