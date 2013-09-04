# think602 Opinions
Bold opinions about how to work.

We believe legalistic structure __kills__. We also believe disciplined but lose 
conventions __enable__ collaborative creativity between many people. We want 
this. The following opinions are specific steps to be __free__, __creative__, 
and __integrated__.


## Table of Contents:

Process Flow:  
- [Branches](#git-branches)  
- [Feature Development](#feature-development)  
- [Pull Requests](#pull-requests)  

Code/Techincal:  
- [HTML](#html)  
- [CSS](#css)  
- [Javascript](#javascript)  
- [iOS](#ios)

<br />
<br />

## Git Branches
Master - always production ready.  
Staging - always staging  ready.  
Features/\* - new/exerpimental code.  
Fixes/\* - bug fixing code.  
Releases - git tag the appropriate branch.  

## Feature Development
Branch from master/staging/etc to `features/<new_feature>` branch. Complete 
feature with tests to cover new code, and pull request into staging.

## Pull Requests
Pull request must contain:  
- new feature code.  
- tests covering code.  
- if code interacts with Frontend, contains or references visual to confirm 
work fulfills visual requirements.  


## HTML

## CSS
Compound words are hyphenated.
  
    #wizard-taxon
    .action-links  

## Javascript

## iOS

### Naming
Use headlessCamelCase (see [wikipedia](http://en.wikipedia.org/wiki/CamelCase)).

### Constants
Application wide constants, 
    
    ### Singletons
    # format
    "app" + "classname"
    
    # example, AFOAuthCredential
    appOauthCredential
    
    ### Keys
    # format
    "k" + "name"
    
    # example
    kEmail
    

### UI IBOutlets and Properties
    
    ### IBOutlet UILabel
    # format
    "classname" + "Object" + "Attribute"
    
    # example
    labelPackageTitle
    
    ### IBOutlet UITableView within UIView
    # format
    "classname" + "Obejcts"
    
    # example 
    tableviewPackages
    
    

### Identifiers
Objective -  know what an identifier is without looking at code.

__UITableView Identifiers__.  
    
    # format
    "cell" + "-" + "name of UIViewController cell appears on" 
    
    # only 1 cell on UIView
    cell-NameOfViewController
    
    # multiple cells on UIView
    cell-NameOfViewController-mainTable
    cell-NameOfViewController-subTable
    
__Seque Identifiers__.  
  
    # format 
    "seque" + "name of ViewController that seque goes to"
    
    # only 1 seque to ViewController
    seque-DestinationViewController
    
    # multiple seques to ViewController
    seque-DesinationViewController-from-OriginatingViewController1
    seque-DesinationViewController-from-OriginatingViewController2

    


<br>
<br>

### Contributions  

### Copyright 
Copyright (c) 2013, Weston Platter. BSD-new.
