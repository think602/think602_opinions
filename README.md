# think602 Opinions
Bold opinions about how we work best.

We believe legalistic structure __kills__. We also believe disciplined but lose 
conventions __enable__ collaborative creativity between many people. We want 
this. The following opinions are specific steps to be __free__, __creative__, 
and __integrated__.


## Table of Contents:

Contracts:  
- [Project Deliverables](#project-deliverables)  

Process Flow:  
- [Branches](#git-branches)  
- [Feature Development](#feature-development)  
- [Pull Requests](#pull-requests)  

Terminology:  
- [User Interface](#user-interface)  

Code/Techincal:  
- [HTML](#html)  
- [CSS](#css)  
- [Javascript](#javascript)  
- [Rails](#rails)  
- [iOS](#ios)  

<br />
<br />

## Project Deliverables
Most clients progressively change project deliverables.  Our usual experience:

1. Sit down the client to understand and agree on project scope and 
deliverables.  Client has few opinions about the finner details of the 
agreed deliverables.

2. Complete and send deliverables back to client for approval.

3. Client requests changes not defined in deliverables.

We understand clients have new ideas, operate in a non-static competitive 
business ecosystem, and therefore need to change strategies and BI/IT 
functionality.  __We value this__. 

 As a [for-profit](http://en.wikipedia.org/wiki/For-profit_corporation) consultancy firm, we have 2 main options, 

1. make changes __without charge__.
2. make changes __charging client standard hourly rate for extra work__.

We operate according #2, IE, charge for undefined work.  Our and others' time is 
limited and we value proactive product management over post project changes.  We 
believe this is disciplined agile development.


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

## User Interface
__display__ - passively create HTML without interpreting substance from which HTML is derived.  
__render__ - actively create HTML by interpreting substance from which HTML is derived as required.  

## HTML

## CSS
Compound words are hyphenated.
  
    #wizard-taxon
    .action-links  

## Javascript

## Rails

### ActiveRecord

    ### chaining multiple methods
    # format
    SomeClass.
      first_method(attribute: 'value').
      second_method.
      third_method(attribute: true)
    
    # example
    @taxon = Spree::Taxon.
        includes(products: { variants: [:images, :default_price, :option_values]}).
        includes(products: { master:   [:images, :default_price, :option_values]}).
        find(params[:taxon_id])

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
    
__StoryBoard Identifiers__.  
    
    # format
    "name of Controller"
    
    # example
    myAudiobooksNav
    myAudiobooks
    myAudiobookDetail
    myAudiobookPackageDetail
    
    
    
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
