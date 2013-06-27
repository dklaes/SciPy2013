  


<!DOCTYPE html>
<html>
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# githubog: http://ogp.me/ns/fb/githubog#">
    <meta charset='utf-8'>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <title>boot-camps/version-control/git/git-and-github/instructor_notes.md at master · swcarpentry/boot-camps · GitHub</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub" />
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub" />
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-114.png" />
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114.png" />
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-144.png" />
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144.png" />
    <link rel="logo" type="image/svg" href="https://github-media-downloads.s3.amazonaws.com/github-logo.svg" />
    <meta property="og:image" content="https://a248.e.akamai.net/assets.github.com/images/modules/logos_page/Octocat.png">
    <link rel="assets" href="https://a248.e.akamai.net/assets.github.com/">
    <link rel="xhr-socket" href="/_sockets" />
    


    <meta name="msapplication-TileImage" content="/windows-tile.png" />
    <meta name="msapplication-TileColor" content="#ffffff" />
    <meta name="selected-link" value="repo_source" data-pjax-transient />
    <meta content="collector.githubapp.com" name="octolytics-host" /><meta content="github" name="octolytics-app-id" />

    
    
    <link rel="icon" type="image/x-icon" href="/favicon.ico" />

    <meta content="authenticity_token" name="csrf-param" />
<meta content="PZjTkJQmjdTv3AYVO1H6zUlWf98kipvC2ua2zBcl3wk=" name="csrf-token" />

    <link href="https://a248.e.akamai.net/assets.github.com/assets/github-c066013be20516a6aae45467044fa109f18bd0c6.css" media="all" rel="stylesheet" type="text/css" />
    <link href="https://a248.e.akamai.net/assets.github.com/assets/github2-08c4405dff2a90b255e2b4849cf2f13937f93993.css" media="all" rel="stylesheet" type="text/css" />
    


      <script src="https://a248.e.akamai.net/assets.github.com/assets/frameworks-8a3b89300fb38cc706e3ed8b1c9d7853a40d9689.js" type="text/javascript"></script>
      <script src="https://a248.e.akamai.net/assets.github.com/assets/github-682bfaa01f5b5de57ebcb71a1f7f8e7840f0523b.js" type="text/javascript"></script>
      
      <meta http-equiv="x-pjax-version" content="79488cdcbd1d3174c6e6f4c98d1c7ef7">

        <link data-pjax-transient rel='permalink' href='/swcarpentry/boot-camps/blob/2b84bd1b5cd63372e975f8d151d665ee9d7edab1/version-control/git/git-and-github/instructor_notes.md'>
    <meta property="og:title" content="boot-camps"/>
    <meta property="og:type" content="githubog:gitrepository"/>
    <meta property="og:url" content="https://github.com/swcarpentry/boot-camps"/>
    <meta property="og:image" content="https://secure.gravatar.com/avatar/d7c59c38273d06899bb322e4b2436b65?s=420&amp;d=https://a248.e.akamai.net/assets.github.com%2Fimages%2Fgravatars%2Fgravatar-user-420.png"/>
    <meta property="og:site_name" content="GitHub"/>
    <meta property="og:description" content="boot-camps - Software Carpentry boot camp material"/>
    <meta property="twitter:card" content="summary"/>
    <meta property="twitter:site" content="@GitHub">
    <meta property="twitter:title" content="swcarpentry/boot-camps"/>

    <meta name="description" content="boot-camps - Software Carpentry boot camp material" />


    <meta content="2238358" name="octolytics-dimension-user_id" /><meta content="swcarpentry" name="octolytics-dimension-user_login" /><meta content="6821320" name="octolytics-dimension-repository_id" /><meta content="swcarpentry/boot-camps" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="6821320" name="octolytics-dimension-repository_network_root_id" /><meta content="swcarpentry/boot-camps" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/swcarpentry/boot-camps/commits/master.atom" rel="alternate" title="Recent Commits to boot-camps:master" type="application/atom+xml" />

  </head>


  <body class="logged_out page-blob  vis-public env-production  ">

    <div class="wrapper">
      
      
      

      
      <div class="header header-logged-out">
  <div class="container clearfix">

    <a class="header-logo-wordmark" href="https://github.com/">
      <span class="mega-octicon octicon-logo-github"></span>
    </a>

    <div class="header-actions">
      <a class="button primary" href="/signup">Sign up</a>
      <a class="button" href="/login?return_to=%2Fswcarpentry%2Fboot-camps%2Fblob%2Fmaster%2Fversion-control%2Fgit%2Fgit-and-github%2Finstructor_notes.md">Sign in</a>
    </div>

    <div class="command-bar js-command-bar  in-repository">


      <ul class="top-nav">
          <li class="explore"><a href="/explore">Explore</a></li>
        <li class="features"><a href="/features">Features</a></li>
          <li class="enterprise"><a href="https://enterprise.github.com/">Enterprise</a></li>
          <li class="blog"><a href="/blog">Blog</a></li>
      </ul>
        <form accept-charset="UTF-8" action="/search" class="command-bar-form" id="top_search_form" method="get">

<input type="text" data-hotkey="/ s" name="q" id="js-command-bar-field" placeholder="Search or type a command" tabindex="1" autocapitalize="off"
    
    
      data-repo="swcarpentry/boot-camps"
      data-branch="master"
      data-sha="ef07b93fd0a051a6ccd2545e42b7e4f7c9d35940"
  >

    <input type="hidden" name="nwo" value="swcarpentry/boot-camps" />

    <div class="select-menu js-menu-container js-select-menu search-context-select-menu">
      <span class="minibutton select-menu-button js-menu-target">
        <span class="js-select-button">This repository</span>
      </span>

      <div class="select-menu-modal-holder js-menu-content js-navigation-container">
        <div class="select-menu-modal">

          <div class="select-menu-item js-navigation-item selected">
            <span class="select-menu-item-icon octicon octicon-check"></span>
            <input type="radio" class="js-search-this-repository" name="search_target" value="repository" checked="checked" />
            <div class="select-menu-item-text js-select-button-text">This repository</div>
          </div> <!-- /.select-menu-item -->

          <div class="select-menu-item js-navigation-item">
            <span class="select-menu-item-icon octicon octicon-check"></span>
            <input type="radio" name="search_target" value="global" />
            <div class="select-menu-item-text js-select-button-text">All repositories</div>
          </div> <!-- /.select-menu-item -->

        </div>
      </div>
    </div>

  <span class="octicon help tooltipped downwards" title="Show command bar help">
    <span class="octicon octicon-question"></span>
  </span>


  <input type="hidden" name="ref" value="cmdform">

</form>
    </div>

  </div>
</div>


      


            <div class="site hfeed" itemscope itemtype="http://schema.org/WebPage">
      <div class="hentry">
        
        <div class="pagehead repohead instapaper_ignore readability-menu ">
          <div class="container">
            <div class="title-actions-bar">
              

<ul class="pagehead-actions">



    <li>
      <a href="/login?return_to=%2Fswcarpentry%2Fboot-camps"
        class="minibutton with-count js-toggler-target star-button entice tooltipped upwards"
        title="You must be signed in to use this feature" rel="nofollow">
        <span class="octicon octicon-star"></span>Star
      </a>
      <a class="social-count js-social-count" href="/swcarpentry/boot-camps/stargazers">
        38
      </a>
    </li>
    <li>
      <a href="/login?return_to=%2Fswcarpentry%2Fboot-camps"
        class="minibutton with-count js-toggler-target fork-button entice tooltipped upwards"
        title="You must be signed in to fork a repository" rel="nofollow">
        <span class="octicon octicon-git-branch"></span>Fork
      </a>
      <a href="/swcarpentry/boot-camps/network" class="social-count">
        215
      </a>
    </li>
</ul>

              <h1 itemscope itemtype="http://data-vocabulary.org/Breadcrumb" class="entry-title public">
                <span class="repo-label"><span>public</span></span>
                <span class="mega-octicon octicon-repo"></span>
                <span class="author vcard">
                  <a href="/swcarpentry" class="url fn" itemprop="url" rel="author">
                  <span itemprop="title">swcarpentry</span>
                  </a></span> /
                <strong><a href="/swcarpentry/boot-camps" class="js-current-repository">boot-camps</a></strong>
              </h1>
            </div>

            
  <ul class="tabs">
    <li class="pulse-nav"><a href="/swcarpentry/boot-camps/pulse" class="js-selected-navigation-item " data-selected-links="pulse /swcarpentry/boot-camps/pulse" rel="nofollow"><span class="octicon octicon-pulse"></span></a></li>
    <li><a href="/swcarpentry/boot-camps" class="js-selected-navigation-item selected" data-selected-links="repo_source repo_downloads repo_commits repo_tags repo_branches /swcarpentry/boot-camps">Code</a></li>
    <li><a href="/swcarpentry/boot-camps/network" class="js-selected-navigation-item " data-selected-links="repo_network /swcarpentry/boot-camps/network">Network</a></li>
    <li><a href="/swcarpentry/boot-camps/pulls" class="js-selected-navigation-item " data-selected-links="repo_pulls /swcarpentry/boot-camps/pulls">Pull Requests <span class='counter'>6</span></a></li>

      <li><a href="/swcarpentry/boot-camps/issues" class="js-selected-navigation-item " data-selected-links="repo_issues /swcarpentry/boot-camps/issues">Issues <span class='counter'>10</span></a></li>

      <li><a href="/swcarpentry/boot-camps/wiki" class="js-selected-navigation-item " data-selected-links="repo_wiki /swcarpentry/boot-camps/wiki">Wiki</a></li>


    <li><a href="/swcarpentry/boot-camps/graphs" class="js-selected-navigation-item " data-selected-links="repo_graphs repo_contributors /swcarpentry/boot-camps/graphs">Graphs</a></li>


  </ul>
  
<div class="tabnav kill-the-chrome-after-repo-next-ship-tabnav">

  <span class="tabnav-right">
    <ul class="tabnav-tabs">
          <li><a href="/swcarpentry/boot-camps/tags" class="js-selected-navigation-item tabnav-tab" data-selected-links="repo_tags /swcarpentry/boot-camps/tags">Tags <span class="counter ">27</span></a></li>
    </ul>
  </span>

  <div class="tabnav-widget scope">


    <div class="select-menu js-menu-container js-select-menu js-branch-menu">
      <a class="minibutton select-menu-button js-menu-target" data-hotkey="w" data-ref="master">
        <span class="octicon octicon-git-branch"></span>
        <i>branch:</i>
        <span class="js-select-button">master</span>
      </a>

      <div class="select-menu-modal-holder js-menu-content js-navigation-container">

        <div class="select-menu-modal">
          <div class="select-menu-header">
            <span class="select-menu-title">Switch branches/tags</span>
            <span class="octicon octicon-remove-close js-menu-close"></span>
          </div> <!-- /.select-menu-header -->

          <div class="select-menu-filters">
            <div class="select-menu-text-filter">
              <input type="text" id="commitish-filter-field" class="js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
            </div>
            <div class="select-menu-tabs">
              <ul>
                <li class="select-menu-tab">
                  <a href="#" data-tab-filter="branches" class="js-select-menu-tab">Branches</a>
                </li>
                <li class="select-menu-tab">
                  <a href="#" data-tab-filter="tags" class="js-select-menu-tab">Tags</a>
                </li>
              </ul>
            </div><!-- /.select-menu-tabs -->
          </div><!-- /.select-menu-filters -->

          <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket css-truncate" data-tab-filter="branches">

            <div data-filterable-for="commitish-filter-field" data-filterable-type="substring">

                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-04-umd/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-04-umd" rel="nofollow" title="2013-04-umd">2013-04-umd</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-05-krakow/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-05-krakow" rel="nofollow" title="2013-05-krakow">2013-05-krakow</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-05-lbl/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-05-lbl" rel="nofollow" title="2013-05-lbl">2013-05-lbl</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-05-nescent/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-05-nescent" rel="nofollow" title="2013-05-nescent">2013-05-nescent</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-05-oxford-dtc/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-05-oxford-dtc" rel="nofollow" title="2013-05-oxford-dtc">2013-05-oxford-dtc</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-05-ucdavis/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-05-ucdavis" rel="nofollow" title="2013-05-ucdavis">2013-05-ucdavis</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-05-umass/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-05-umass" rel="nofollow" title="2013-05-umass">2013-05-umass</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-06-chicago/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-06-chicago" rel="nofollow" title="2013-06-chicago">2013-06-chicago</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-06-dssg/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-06-dssg" rel="nofollow" title="2013-06-dssg">2013-06-dssg</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-06-southampton/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-06-southampton" rel="nofollow" title="2013-06-southampton">2013-06-southampton</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-06-tufts/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-06-tufts" rel="nofollow" title="2013-06-tufts">2013-06-tufts</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-06-wise-advanced/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-06-wise-advanced" rel="nofollow" title="2013-06-wise-advanced">2013-06-wise-advanced</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-06-wise-beginners/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-06-wise-beginners" rel="nofollow" title="2013-06-wise-beginners">2013-06-wise-beginners</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-06-wise-intermediate/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-06-wise-intermediate" rel="nofollow" title="2013-06-wise-intermediate">2013-06-wise-intermediate</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-07-11-iub/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-07-11-iub" rel="nofollow" title="2013-07-11-iub">2013-07-11-iub</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-07-bath/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-07-bath" rel="nofollow" title="2013-07-bath">2013-07-bath</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-07-oslo/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-07-oslo" rel="nofollow" title="2013-07-oslo">2013-07-oslo</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-10-cambs-r/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-10-cambs-r" rel="nofollow" title="2013-10-cambs-r">2013-10-cambs-r</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/gh-pages/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="gh-pages" rel="nofollow" title="gh-pages">gh-pages</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item selected">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/master/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="master" rel="nofollow" title="master">master</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/tufts/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="tufts" rel="nofollow" title="tufts">tufts</a>
                </div> <!-- /.select-menu-item -->
            </div>

              <div class="select-menu-no-results">Nothing to show</div>
          </div> <!-- /.select-menu-list -->


          <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket css-truncate" data-tab-filter="tags">
            <div data-filterable-for="commitish-filter-field" data-filterable-type="substring">

                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/hackerwith-trieste-solution/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="hackerwith-trieste-solution" rel="nofollow" title="hackerwith-trieste-solution">hackerwith-trieste-solution</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/hackerwith-trieste-master/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="hackerwith-trieste-master" rel="nofollow" title="hackerwith-trieste-master">hackerwith-trieste-master</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-05-06-stanford/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-05-06-stanford" rel="nofollow" title="2013-05-06-stanford">2013-05-06-stanford</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-04-ucb/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-04-ucb" rel="nofollow" title="2013-04-ucb">2013-04-ucb</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-04-manchester/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-04-manchester" rel="nofollow" title="2013-04-manchester">2013-04-manchester</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-04-egi-forum/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-04-egi-forum" rel="nofollow" title="2013-04-egi-forum">2013-04-egi-forum</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-03-lbl-2/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-03-lbl-2" rel="nofollow" title="2013-03-lbl-2">2013-03-lbl-2</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-02-uwash-B/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-02-uwash-B" rel="nofollow" title="2013-02-uwash-B">2013-02-uwash-B</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-02-uwash-A/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-02-uwash-A" rel="nofollow" title="2013-02-uwash-A">2013-02-uwash-A</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-01-columbia/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-01-columbia" rel="nofollow" title="2013-01-columbia">2013-01-columbia</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2013-01-chicago/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2013-01-chicago" rel="nofollow" title="2013-01-chicago">2013-01-chicago</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2012-12-edinburgh/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2012-12-edinburgh" rel="nofollow" title="2012-12-edinburgh">2012-12-edinburgh</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2012-12-austin/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2012-12-austin" rel="nofollow" title="2012-12-austin">2012-12-austin</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2012-11-unc/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2012-11-unc" rel="nofollow" title="2012-11-unc">2012-11-unc</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2012-11-uh/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2012-11-uh" rel="nofollow" title="2012-11-uh">2012-11-uh</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2012-11-scripps/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2012-11-scripps" rel="nofollow" title="2012-11-scripps">2012-11-scripps</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2012-10-ucb/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2012-10-ucb" rel="nofollow" title="2012-10-ucb">2012-10-ucb</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2012-10-purdue/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2012-10-purdue" rel="nofollow" title="2012-10-purdue">2012-10-purdue</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2012-10-oxford/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2012-10-oxford" rel="nofollow" title="2012-10-oxford">2012-10-oxford</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2012-10-newcastle/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2012-10-newcastle" rel="nofollow" title="2012-10-newcastle">2012-10-newcastle</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2012-10-lbl/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2012-10-lbl" rel="nofollow" title="2012-10-lbl">2012-10-lbl</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2012-10-gmu/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2012-10-gmu" rel="nofollow" title="2012-10-gmu">2012-10-gmu</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2012-10-caltech/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2012-10-caltech" rel="nofollow" title="2012-10-caltech">2012-10-caltech</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2012-06-jhu/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2012-06-jhu" rel="nofollow" title="2012-06-jhu">2012-06-jhu</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2012-06-inria/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2012-06-inria" rel="nofollow" title="2012-06-inria">2012-06-inria</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2012-05-newcastle/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2012-05-newcastle" rel="nofollow" title="2012-05-newcastle">2012-05-newcastle</a>
                </div> <!-- /.select-menu-item -->
                <div class="select-menu-item js-navigation-item ">
                  <span class="select-menu-item-icon octicon octicon-check"></span>
                  <a href="/swcarpentry/boot-camps/blob/2012-04-uchicago/version-control/git/git-and-github/instructor_notes.md" class="js-navigation-open select-menu-item-text js-select-button-text css-truncate-target" data-name="2012-04-uchicago" rel="nofollow" title="2012-04-uchicago">2012-04-uchicago</a>
                </div> <!-- /.select-menu-item -->
            </div>

            <div class="select-menu-no-results">Nothing to show</div>

          </div> <!-- /.select-menu-list -->

        </div> <!-- /.select-menu-modal -->
      </div> <!-- /.select-menu-modal-holder -->
    </div> <!-- /.select-menu -->

  </div> <!-- /.scope -->

  <ul class="tabnav-tabs">
    <li><a href="/swcarpentry/boot-camps" class="selected js-selected-navigation-item tabnav-tab" data-selected-links="repo_source /swcarpentry/boot-camps">Files</a></li>
    <li><a href="/swcarpentry/boot-camps/commits/master" class="js-selected-navigation-item tabnav-tab" data-selected-links="repo_commits /swcarpentry/boot-camps/commits/master">Commits</a></li>
    <li><a href="/swcarpentry/boot-camps/branches" class="js-selected-navigation-item tabnav-tab" data-selected-links="repo_branches /swcarpentry/boot-camps/branches" rel="nofollow">Branches <span class="counter ">21</span></a></li>
  </ul>

</div>

  


            
          </div>
        </div><!-- /.repohead -->

        <div id="js-repo-pjax-container" class="container context-loader-container" data-pjax-container>
          


<!-- blob contrib key: blob_contributors:v21:bf880f3015e9803db8e0bbd62975ea0e -->
<!-- blob contrib frag key: views10/v8/blob_contributors:v21:bf880f3015e9803db8e0bbd62975ea0e -->

<div id="slider">
    <div class="frame-meta">

      <p title="This is a placeholder element" class="js-history-link-replace hidden"></p>

        <a href="/swcarpentry/boot-camps/find/master" class="js-slide-to" data-hotkey="t" style="display:none">Show File Finder</a>

        <div class="breadcrumb">
          <span class='repo-root js-repo-root'><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/swcarpentry/boot-camps" class="js-slide-to" data-branch="master" data-direction="back" itemscope="url"><span itemprop="title">boot-camps</span></a></span></span><span class="separator"> / </span><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/swcarpentry/boot-camps/tree/master/version-control" class="js-slide-to" data-branch="master" data-direction="back" itemscope="url"><span itemprop="title">version-control</span></a></span><span class="separator"> / </span><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/swcarpentry/boot-camps/tree/master/version-control/git" class="js-slide-to" data-branch="master" data-direction="back" itemscope="url"><span itemprop="title">git</span></a></span><span class="separator"> / </span><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/swcarpentry/boot-camps/tree/master/version-control/git/git-and-github" class="js-slide-to" data-branch="master" data-direction="back" itemscope="url"><span itemprop="title">git-and-github</span></a></span><span class="separator"> / </span><strong class="final-path">instructor_notes.md</strong> <span class="js-zeroclipboard zeroclipboard-button" data-clipboard-text="version-control/git/git-and-github/instructor_notes.md" data-copied-hint="copied!" title="copy to clipboard"><span class="octicon octicon-clippy"></span></span>
        </div>


        
  <div class="commit file-history-tease">
    <img class="main-avatar" height="24" src="https://secure.gravatar.com/avatar/3994f17d0e03f2587d9fd2b7e5187fa8?s=140&amp;d=https://a248.e.akamai.net/assets.github.com%2Fimages%2Fgravatars%2Fgravatar-user-420.png" width="24" />
    <span class="author"><a href="/jiffyclub" rel="author">jiffyclub</a></span>
    <time class="js-relative-date" datetime="2013-03-05T06:50:55-08:00" title="2013-03-05 06:50:55">March 05, 2013</time>
    <div class="commit-title">
        <a href="/swcarpentry/boot-camps/commit/e444c09ccd74d8ac993c89a75178e233bddad6f9" class="message" data-pjax="true">Instructor notes for teaching git via collaboration on GitHub.</a>
    </div>

    <div class="participation">
      <p class="quickstat"><a href="#blob_contributors_box" rel="facebox"><strong>1</strong> contributor</a></p>
      
    </div>
    <div id="blob_contributors_box" style="display:none">
      <h2 class="facebox-header">Users who have contributed to this file</h2>
      <ul class="facebox-user-list">
        <li class="facebox-user-list-item">
          <img height="24" src="https://secure.gravatar.com/avatar/3994f17d0e03f2587d9fd2b7e5187fa8?s=140&amp;d=https://a248.e.akamai.net/assets.github.com%2Fimages%2Fgravatars%2Fgravatar-user-420.png" width="24" />
          <a href="/jiffyclub">jiffyclub</a>
        </li>
      </ul>
    </div>
  </div>


    </div><!-- ./.frame-meta -->

    <div class="frames">
      <div class="frame" data-permalink-url="/swcarpentry/boot-camps/blob/2b84bd1b5cd63372e975f8d151d665ee9d7edab1/version-control/git/git-and-github/instructor_notes.md" data-title="boot-camps/version-control/git/git-and-github/instructor_notes.md at master · swcarpentry/boot-camps · GitHub" data-type="blob">

        <div id="files" class="bubble">
          <div class="file">
            <div class="meta">
              <div class="info">
                <span class="icon"><b class="octicon octicon-file-text"></b></span>
                <span class="mode" title="File Mode">file</span>
                  <span>248 lines (196 sloc)</span>
                <span>10.084 kb</span>
              </div>
              <div class="actions">
                <div class="button-group">
                      <a class="minibutton js-entice" href=""
                         data-entice="You must be signed in and on a branch to make or propose changes">Edit</a>
                  <a href="/swcarpentry/boot-camps/raw/master/version-control/git/git-and-github/instructor_notes.md" class="button minibutton " id="raw-url">Raw</a>
                    <a href="/swcarpentry/boot-camps/blame/master/version-control/git/git-and-github/instructor_notes.md" class="button minibutton ">Blame</a>
                  <a href="/swcarpentry/boot-camps/commits/master/version-control/git/git-and-github/instructor_notes.md" class="button minibutton " rel="nofollow">History</a>
                </div><!-- /.button-group -->
              </div><!-- /.actions -->

            </div>
              
  <div id="readme" class="blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="mainContentOfPage"><h1>
<a name="gitgithub" class="anchor" href="#gitgithub"><span class="octicon octicon-link"></span></a>git/GitHub</h1>

<p>The goal of this lesson is to introduce the students to <a href="http://git-scm.com/">git</a> via
collaboration on <a href="http://github.com">GitHub</a>.</p>

<h2>
<a name="introduction" class="anchor" href="#introduction"><span class="octicon octicon-link"></span></a>Introduction</h2>

<ul>
<li>Say some introductory stuff about version control in general, and git/GitHub
in particular.</li>
</ul><p><em>Note: The figures in the <a href="http://marklodato.github.com/visual-git-guide/index-en.html">Visual Git Reference</a> can be a good
stand-in if you have nowhere to draw.</em></p>

<h2>
<a name="setup-and-signup" class="anchor" href="#setup-and-signup"><span class="octicon octicon-link"></span></a>Setup and Signup</h2>

<ul>
<li>
<p>Have everyone configure git:</p>

<pre><code>$ git config --global user.name "User Name"
$ git config --global user.email "user@email.com"
$ git config --global core.editor "nano"
$ git config --global color.ui "auto"
</code></pre>
</li>
<li><p>Give a little tour of <a href="http://github.com">GitHub</a>.</p></li>
<li><p>Have everyone make <a href="http://github.com">GitHub</a> accounts.</p></li>
</ul><h3>
<a name="make-and-clone" class="anchor" href="#make-and-clone"><span class="octicon octicon-link"></span></a>Make and Clone</h3>

<ul>
<li>Make a new demo repo on <a href="http://github.com">GitHub</a> explaining the process as you go
(probably on your personal account).

<ul>
<li>Have <a href="http://github.com">GitHub</a> put in a README so it can be cloned.</li>
</ul>
</li>
<li>Explain that much like a browser navigates to websites using a URL, git talks
to remote repositories using a URL.</li>
<li>Explain the different URL options:

<ul>
<li>Read/write <code>ssh</code> protocol requires <a href="https://help.github.com/articles/generating-ssh-keys">ssh keys</a>, which make it so you
don't have to enter username/password.</li>
<li>
<code>https</code> protocol takes username/password.</li>
<li>
<code>git</code> protocol is read-only.</li>
</ul>
</li>
<li>Now we want to get a copy of this down on all of our computers -- <code>git clone</code>!

<ul>
<li>Have everyone do this via the <code>https</code> URL.</li>
</ul>
</li>
<li>
<code>ls</code> to show the new directory and <code>cd</code> into it.</li>
<li>Compare the local listing to what you see on <a href="http://github.com">GitHub</a>. Same for now, but
not for long!</li>
</ul><h2>
<a name="basics" class="anchor" href="#basics"><span class="octicon octicon-link"></span></a>Basics</h2>

<h3>
<a name="local-basics" class="anchor" href="#local-basics"><span class="octicon octicon-link"></span></a>Local Basics</h3>

<p><strong>IMPORTANT:</strong> Make sure you tell people <em>not</em> to make their own local changes,
that will make things really complicated later when people pull. Alternatively,
you can go ahead and let them do whatever they like and use it as a teaching
moment on <code>git reset --hard</code> in a few minutes when it's time to start the
collaboration.</p>

<ul>
<li>On the white board draw a box representing the working area and explain that
this is where you work and make changes.</li>
<li>Make a new file called <code>top-things-to-learn.md</code> and put the title
"Top Things We Want to Learn" in it.</li>
<li>
<code>git status</code> -- highlight the "Untracked files" section and that git tells
you how to add a file to the next commit.</li>
</ul><h3>
<a name="composing-the-snapshot" class="anchor" href="#composing-the-snapshot"><span class="octicon octicon-link"></span></a>Composing the Snapshot</h3>

<ul>
<li>On the white board draw a box representing the staging area (index) and
explain that this is where we set up the next snapshot of our project.

<ul>
<li>Like a photographer in a studio, we're putting together a shot before
we actually snap the picture.</li>
<li>Connect the working area box and the staging box with <code>git add</code>.</li>
</ul>
</li>
<li>Run <code>git add top-things-to-learn.md</code>.</li>
<li>
<code>git status</code> -- highlight the "Changes to be committed" section
and git telling you how to unstage the new file.</li>
</ul><h3>
<a name="taking-the-snapshot" class="anchor" href="#taking-the-snapshot"><span class="octicon octicon-link"></span></a>Taking the Snapshot</h3>

<ul>
<li>On the white board draw a box representing the project history. Once we take
a snapshot of the project that snapshot becomes a permanent reference point
in the project's history that we can always go back to.

<ul>
<li>The history is like a photo album of changes, and each snapshot has a
time stamp, the name of the photographer, and a description.</li>
<li>Connect the staging area to the history with <code>git commit</code>.</li>
</ul>
</li>
<li>Run <code>git commit</code> and explain log messages.

<ul>
<li>Summary message at the top, longer one below.</li>
</ul>
</li>
<li>
<code>git status</code> -- nothing going on!</li>
</ul><h3>
<a name="looking-at-the-history" class="anchor" href="#looking-at-the-history"><span class="octicon octicon-link"></span></a>Looking at the History</h3>

<ul>
<li>
<code>git log</code> -- Shows description of what we've done.

<ul>
<li>
<code>git log --oneline</code> -- Abbreviated version.</li>
</ul>
</li>
<li>Explain the commit hash.

<ul>
<li>Unique identifier of that commit if we ever want to refer to it.</li>
<li>Comes from "hashing" stuff associated with the commit, like the changes
we made.</li>
<li>Can demo hashing with Python's <code>hashlib.sha1</code>.</li>
</ul>
</li>
</ul><h3>
<a name="previewing-changes" class="anchor" href="#previewing-changes"><span class="octicon octicon-link"></span></a>Previewing Changes</h3>

<ul>
<li>The file we're making is going to be a list of the top things everyone wants
to learn in the boot camp. Add your item (e.g. everyone's names) and save.</li>
<li>
<code>git status</code> -- point out that now we have a modified file instead of an
untracked file, but the procedure for adding it to the next snapshot is
the same.</li>
<li>Want to see the changes you're about to add? <code>git diff</code>!</li>
<li><code>git add</code></li>
<li>
<code>git diff</code> -- now it doesn't show anything. <code>git diff</code> shows differences
between the working area and the staging area.

<ul>
<li>To see differences between the staging area and the most recent commit
use <code>git diff --cached</code>.</li>
</ul>
</li>
<li>
<code>git commit -m</code> -- This time use the <code>-m</code> option and show that for short
commit messages you can just enter them at the command line.</li>
</ul><h3>
<a name="undoing-changes" class="anchor" href="#undoing-changes"><span class="octicon octicon-link"></span></a>Undoing Changes</h3>

<ul>
<li>Say I want to redo the previous commit...</li>
<li>
<code>git log --oneline</code> -- grab the commit has for the point we want to go back to.</li>
<li><code>git reset COMMIT</code></li>
<li>
<code>git log --oneline</code> -- highlight that the latest commit is gone</li>
<li>
<code>git status</code> -- But the changes haven't gone anywhere.</li>
<li>I can now edit the file to fix whatever was wrong and re-commit.</li>
</ul><h2>
<a name="sharing" class="anchor" href="#sharing"><span class="octicon octicon-link"></span></a>Sharing</h2>

<ul>
<li>Now I want to share my changes with everyone so they can start working on
it too.</li>
</ul><h3>
<a name="remotes" class="anchor" href="#remotes"><span class="octicon octicon-link"></span></a>Remotes</h3>

<ul>
<li>As we said back at the beginning, git uses URLs to point repositories on other
computers, in this case <a href="http://github.com">GitHub's</a> servers.</li>
<li>We can give these remote repositories names so that we don't have to type
in the full URL all the time, and in fact git has already set one up for us.</li>
<li>
<code>git remote</code> -- there's a remote called "origin".</li>
<li>
<code>git remote -v</code> -- we can see that it points to the same URL we cloned from,
git sets this up automatically.</li>
</ul><h3>
<a name="branches" class="anchor" href="#branches"><span class="octicon octicon-link"></span></a>Branches</h3>

<ul>
<li>On the <a href="http://github.com">GitHub</a> view of the repo highlight the branches pull-down -- right
now it only has one branch called "master", this is another thing git makes
for us by default.</li>
<li>What branch are we on locally? <code>git branch</code>.</li>
<li>Give a short explanation of branches and mention that we will come back to
them later.

<ul>
<li>Isolated development environments.</li>
</ul>
</li>
<li>When git communicates with a remote repository it needs to know what branch
is changing, in this case we'll just stick with "master".</li>
</ul><h3>
<a name="pushing" class="anchor" href="#pushing"><span class="octicon octicon-link"></span></a>Pushing</h3>

<ul>
<li>Use <code>push</code> command to send data to a remote repository, and we also have to
specify the remote name and branch name: <code>git push origin master</code>.</li>
<li>Refresh the <a href="http://github.com">GitHub</a> view.</li>
</ul><h3>
<a name="pulling" class="anchor" href="#pulling"><span class="octicon octicon-link"></span></a>Pulling</h3>

<p><strong>IMPORTANT:</strong> If students have been making local commits, this is the time at
which they will need to use <code>git reset --hard</code> to get back in sync with you.</p>

<ul>
<li>
<code>pull</code> is the reciprocal command, must specify remote and branch.</li>
<li>Have everyone <code>git pull origin master</code>.</li>
</ul><h3>
<a name="collaborate" class="anchor" href="#collaborate"><span class="octicon octicon-link"></span></a>Collaborate</h3>

<ul>
<li>Pick a student to add their top thing to learn to the list:

<ul>
<li>Add them to the collaborator list on the demo repo.</li>
<li>edit, save, <code>add</code>, <code>commit</code>, <code>push</code>
</li>
</ul>
</li>
<li>Have everyone <code>pull</code>.</li>
</ul><h3>
<a name="rebase" class="anchor" href="#rebase"><span class="octicon octicon-link"></span></a>Rebase</h3>

<h4>
<a name="no-conflict" class="anchor" href="#no-conflict"><span class="octicon octicon-link"></span></a>No Conflict</h4>

<ul>
<li>Have another student add their thing and push.</li>
<li>Make a change to the README file before pulling.</li>
<li>Try to push.</li>
<li>On the white board draw the situation: my repo and the remote repo have
different development histories and git doesn't know how to pull things
together.</li>
<li>It would be nice if I could move my local change after the remote change.
(Draw picture.) There's a command for that!</li>
<li>
<code>git fetch origin</code> -- This gets information from the remote repository
but doesn't integrate it with your local repo like <code>pull</code> does.</li>
<li>
<code>git rebase origin/master</code> -- <code>origin/master</code> is how we specify the fetched
data for the remote named "origin" and it's branch named "master".

<ul>
<li>This replays my local changes on top of the state of the remote repo.</li>
</ul>
</li>
<li>
<code>git log --oneline</code> -- Now my change is after the remote change.</li>
<li><code>git push origin master</code></li>
<li>Have everyone pull.</li>
</ul><h4>
<a name="with-conflicts" class="anchor" href="#with-conflicts"><span class="octicon octicon-link"></span></a>With Conflicts</h4>

<ul>
<li>Again, have a student add their thing and push.</li>
<li>Before pulling make a change in the same place in the same file.</li>
<li>Try to rebase as above.</li>
<li>Explain the conflict message git prints out.</li>
<li>Show the conflict messages in the file and how to clean it up.</li>
<li>Continue the rebase and push the result.</li>
<li>Have everyone pull.</li>
</ul><h2>
<a name="developing-in-branches" class="anchor" href="#developing-in-branches"><span class="octicon octicon-link"></span></a>Developing in Branches</h2>

<p>Often you want to leave a stable version of your code alone while you make some
potentially disruptive changes. Or you and someone else are working on the code
and you want to be able to work without worrying what others are doing.</p>

<ul>
<li>It's going to take a long time to get everyone's top thing to learn onto the
list one at a time, so the room is going to break out into groups and each
come up with their own list.</li>
<li>So that they can all do this and then push their result to <a href="http://github.com">GitHub</a> each
is going to work in their own, isolated branch.</li>
</ul><h3>
<a name="making-a-new-branch" class="anchor" href="#making-a-new-branch"><span class="octicon octicon-link"></span></a>Making a New Branch</h3>

<p><em>Note: The <a href="http://pcottle.github.com/learnGitBranching/?NODEMO">Learn Git Branching</a> app can be a useful way to
illustrate this part of the lesson.</em></p>

<ul>
<li>Make a new branch: <code>git branch matt-list</code>.</li>
<li>
<code>git branch</code> -- highlight the asterisk showing the branch we're currently on.</li>
<li>Move to that branch: <code>git checkout matt-list</code>.</li>
<li>
<code>git branch</code> -- asterisk moved!</li>
<li>Make a change and push.

<ul>
<li>
<strong>IMPORTANT:</strong> have to specify new branch named when pushing, not "master".</li>
</ul>
</li>
<li>
<code>git checkout master</code> -- show that your change is <em>not</em> in master.</li>
<li>Show how to browse to the other branch on <a href="http://github.com">GitHub</a>.</li>
<li>Have each group pick a unique branch name, switch to that branch, and add
all of their top things to learn to the list and push the result.</li>
</ul><h3>
<a name="resolving-the-changes" class="anchor" href="#resolving-the-changes"><span class="octicon octicon-link"></span></a>Resolving the Changes</h3>

<ul>
<li>Browse all of the new branches on <a href="http://github.com">GitHub</a>.</li>
<li>Illustrate the situation on the <a href="http://pcottle.github.com/learnGitBranching/?NODEMO">Learn Git Branching</a> app.</li>
<li>Could just pick one of these branches as the new one "master" and move on,
but we're more adventurous than that.</li>
<li>Make sure you're in "master".</li>
<li>
<code>git fetch origin</code> -- without a branch name it grabs all of the new branches.</li>
<li>Pick a branch and <code>git merge branch-name</code>.

<ul>
<li>Should be a smooth fast-forward.</li>
<li>Illustrate on the <a href="http://pcottle.github.com/learnGitBranching/?NODEMO">Learn Git Branching</a> app.</li>
</ul>
</li>
<li>Pick another branch and try to merge.

<ul>
<li>Resolve conflicts, add, and commit.</li>
<li>Illustrate on the <a href="http://pcottle.github.com/learnGitBranching/?NODEMO">Learn Git Branching</a> app.</li>
</ul>
</li>
<li>Repeat as necessary.</li>
<li>Push the final result to <a href="http://github.com">GitHub</a>.</li>
</ul></article>
  </div>

          </div>
        </div>

        <a href="#jump-to-line" rel="facebox[.linejump]" data-hotkey="l" class="js-jump-to-line" style="display:none">Jump to Line</a>
        <div id="jump-to-line" style="display:none">
          <form accept-charset="UTF-8" class="js-jump-to-line-form">
            <input class="linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;">
            <button type="submit" class="button">Go</button>
          </form>
        </div>

      </div>
    </div>
</div>

<div id="js-frame-loading-template" class="frame frame-loading large-loading-area" style="display:none;">
  <img class="js-frame-loading-spinner" src="https://a248.e.akamai.net/assets.github.com/images/spinners/octocat-spinner-128.gif" height="64" width="64">
</div>


        </div>
      </div>
      <div class="modal-backdrop"></div>
    </div>

    </div><!-- /.wrapper -->

      <div class="container">
  <div class="site-footer">
    <ul class="site-footer-links right">
      <li><a href="https://status.github.com/">Status</a></li>
      <li><a href="http://developer.github.com">Developer</a></li>
      <li><a href="http://training.github.com">Training</a></li>
      <li><a href="http://shop.github.com">Shop</a></li>
      <li><a href="/blog">Blog</a></li>
      <li><a href="/about">About</a></li>
    </ul>

    <a href="/">
      <span class="mega-octicon octicon-mark-github"></span>
    </a>

    <ul class="site-footer-links">
      <li>&copy; 2013 <span title="0.16854s from fe4.rs.github.com">GitHub</span>, Inc.</li>
        <li><a href="/site/terms">Terms</a></li>
        <li><a href="/site/privacy">Privacy</a></li>
        <li><a href="/security">Security</a></li>
        <li><a href="/contact">Contact</a></li>
    </ul>
  </div><!-- /.site-footer -->
</div><!-- /.container -->


    <div class="fullscreen-overlay js-fullscreen-overlay" id="fullscreen_overlay">
  <div class="fullscreen-container js-fullscreen-container">
    <div class="textarea-wrap">
      <textarea name="fullscreen-contents" id="fullscreen-contents" class="js-fullscreen-contents" placeholder="" data-suggester="fullscreen_suggester"></textarea>
          <div class="suggester-container">
              <div class="suggester fullscreen-suggester js-navigation-container" id="fullscreen_suggester"
                 data-url="/swcarpentry/boot-camps/suggestions/commit">
              </div>
          </div>
    </div>
  </div>
  <div class="fullscreen-sidebar">
    <a href="#" class="exit-fullscreen js-exit-fullscreen tooltipped leftwards" title="Exit Zen Mode">
      <span class="mega-octicon octicon-screen-normal"></span>
    </a>
    <a href="#" class="theme-switcher js-theme-switcher tooltipped leftwards"
      title="Switch themes">
      <span class="octicon octicon-color-mode"></span>
    </a>
  </div>
</div>



    <div id="ajax-error-message" class="flash flash-error">
      <span class="octicon octicon-alert"></span>
      <a href="#" class="octicon octicon-remove-close close ajax-error-dismiss"></a>
      Something went wrong with that request. Please try again.
    </div>

    
    <span id='server_response_time' data-time='0.16894' data-host='fe4'></span>
    
  </body>
</html>

