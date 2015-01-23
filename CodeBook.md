



<!DOCTYPE html>
<html lang="en" class="">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    
    
    <title>coursera-tidy-data/CodeBook.md at master · bpoweski/coursera-tidy-data</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-144.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="bpoweski/coursera-tidy-data" name="twitter:title" /><meta content="Contribute to coursera-tidy-data development by creating an account on GitHub." name="twitter:description" /><meta content="https://avatars1.githubusercontent.com/u/103650?v=3&amp;s=400" name="twitter:image:src" />
<meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="https://avatars1.githubusercontent.com/u/103650?v=3&amp;s=400" property="og:image" /><meta content="bpoweski/coursera-tidy-data" property="og:title" /><meta content="https://github.com/bpoweski/coursera-tidy-data" property="og:url" /><meta content="Contribute to coursera-tidy-data development by creating an account on GitHub." property="og:description" />

      <meta name="browser-stats-url" content="/_stats">
    <link rel="assets" href="https://assets-cdn.github.com/">
    <link rel="conduit-xhr" href="https://ghconduit.com:25035">
    <link rel="xhr-socket" href="/_sockets">
    <meta name="pjax-timeout" content="1000">
    <link rel="sudo-modal" href="/sessions/sudo_modal">

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>
      <meta name="google-analytics" content="UA-3769691-2">

    <meta content="collector.githubapp.com" name="octolytics-host" /><meta content="collector-cdn.github.com" name="octolytics-script-host" /><meta content="github" name="octolytics-app-id" /><meta content="47DED0BB:1672:688427B:54C1EBEF" name="octolytics-dimension-request_id" /><meta content="8109116" name="octolytics-actor-id" /><meta content="sanju-bhogvan" name="octolytics-actor-login" /><meta content="1f2ed804cbd4141842a4114b01b1745ff55876d662013050bfe712625fa0edcf" name="octolytics-actor-hash" />
    
    <meta content="Rails, view, blob#show" name="analytics-event" />

    
    
    <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">


    <meta content="authenticity_token" name="csrf-param" />
<meta content="ppsYKkXE0QVbrrZP0CY1VHmzSgS33+JK/1KSdQGLrjw9fPhX6yTqQRfQik4JKQVWIfkuDi9JbOlfegB00xKP9Q==" name="csrf-token" />

    <link href="https://assets-cdn.github.com/assets/github-3b24b9ac37e087c9b13ad8d84820250a93a4fd610eb6e7535e8b12d0cb87836d.css" media="all" rel="stylesheet" type="text/css" />
    <link href="https://assets-cdn.github.com/assets/github2-0adb277c3e0f5609666d7512f78f267969a5308b562c1ff52296b9f0502ae547.css" media="all" rel="stylesheet" type="text/css" />
    
    


    <meta http-equiv="x-pjax-version" content="596976bda9133448b226ab995e1baeb1">

      
  <meta name="description" content="Contribute to coursera-tidy-data development by creating an account on GitHub.">
  <meta name="go-import" content="github.com/bpoweski/coursera-tidy-data git https://github.com/bpoweski/coursera-tidy-data.git">

  <meta content="103650" name="octolytics-dimension-user_id" /><meta content="bpoweski" name="octolytics-dimension-user_login" /><meta content="19219512" name="octolytics-dimension-repository_id" /><meta content="bpoweski/coursera-tidy-data" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="19219512" name="octolytics-dimension-repository_network_root_id" /><meta content="bpoweski/coursera-tidy-data" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/bpoweski/coursera-tidy-data/commits/master.atom" rel="alternate" title="Recent Commits to coursera-tidy-data:master" type="application/atom+xml">

  </head>


  <body class="logged_in  env-production windows vis-public page-blob">
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>
    <div class="wrapper">
      
      
      
      


      <div class="header header-logged-in true" role="banner">
  <div class="container clearfix">

    <a class="header-logo-invertocat" href="https://github.com/" data-hotkey="g d" aria-label="Homepage" ga-data-click="Header, go to dashboard, icon:logo">
  <span class="mega-octicon octicon-mark-github"></span>
</a>


      <div class="site-search repo-scope js-site-search" role="search">
          <form accept-charset="UTF-8" action="/bpoweski/coursera-tidy-data/search" class="js-site-search-form" data-global-search-url="/search" data-repo-search-url="/bpoweski/coursera-tidy-data/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
  <input type="text"
    class="js-site-search-field is-clearable"
    data-hotkey="s"
    name="q"
    placeholder="Search"
    data-global-scope-placeholder="Search GitHub"
    data-repo-scope-placeholder="Search"
    tabindex="1"
    autocapitalize="off">
  <div class="scope-badge">This repository</div>
</form>
      </div>
      <ul class="header-nav left" role="navigation">
        <li class="header-nav-item explore">
          <a class="header-nav-link" href="/explore" data-ga-click="Header, go to explore, text:explore">Explore</a>
        </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="https://gist.github.com" data-ga-click="Header, go to gist, text:gist">Gist</a>
          </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="/blog" data-ga-click="Header, go to blog, text:blog">Blog</a>
          </li>
        <li class="header-nav-item">
          <a class="header-nav-link" href="https://help.github.com" data-ga-click="Header, go to help, text:help">Help</a>
        </li>
      </ul>

    
<ul class="header-nav user-nav right" id="user-links">
  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link name" href="/sanju-bhogvan" data-ga-click="Header, go to profile, text:username">
      <img alt="sanju-bhogvan" class="avatar" data-user="8109116" height="20" src="https://avatars0.githubusercontent.com/u/8109116?v=3&amp;s=40" width="20" />
      <span class="css-truncate">
        <span class="css-truncate-target">sanju-bhogvan</span>
      </span>
    </a>
  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link js-menu-target tooltipped tooltipped-s" href="#" aria-label="Create new..." data-ga-click="Header, create new, icon:add">
      <span class="octicon octicon-plus"></span>
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      
<ul class="dropdown-menu">
  <li>
    <a href="/new" data-ga-click="Header, create new repository, icon:repo"><span class="octicon octicon-repo"></span> New repository</a>
  </li>
  <li>
    <a href="/organizations/new" data-ga-click="Header, create new organization, icon:organization"><span class="octicon octicon-organization"></span> New organization</a>
  </li>


    <li class="dropdown-divider"></li>
    <li class="dropdown-header">
      <span title="bpoweski/coursera-tidy-data">This repository</span>
    </li>
      <li>
        <a href="/bpoweski/coursera-tidy-data/issues/new" data-ga-click="Header, create new issue, icon:issue"><span class="octicon octicon-issue-opened"></span> New issue</a>
      </li>
</ul>

    </div>
  </li>

  <li class="header-nav-item">
        <a href="/notifications" aria-label="You have no unread notifications" class="header-nav-link notification-indicator tooltipped tooltipped-s" data-ga-click="Header, go to notifications, icon:read" data-hotkey="g n">
        <span class="mail-status all-read"></span>
        <span class="octicon octicon-inbox"></span>
</a>
  </li>

  <li class="header-nav-item">
    <a class="header-nav-link tooltipped tooltipped-s" href="/settings/profile" id="account_settings" aria-label="Settings" data-ga-click="Header, go to settings, icon:settings">
      <span class="octicon octicon-gear"></span>
    </a>
  </li>

  <li class="header-nav-item">
    <form accept-charset="UTF-8" action="/logout" class="logout-form" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="bZW6NDlg6un+Q2hruEUP2W0t2RsCn12keQsm7+CkAx4OLnGRJmrvyLdPpag+04PIhCbI13DCNnrCqPwDg3UwOA==" /></div>
      <button class="header-nav-link sign-out-button tooltipped tooltipped-s" aria-label="Sign out" data-ga-click="Header, sign out, icon:logout">
        <span class="octicon octicon-sign-out"></span>
      </button>
</form>  </li>

</ul>


    
  </div>
</div>

      

        
<div class="flash-global js-notice flash-warn">
<div class="container">
    <h2>
      You don't have any verified emails.  We recommend <a href="https://github.com/settings/emails">verifying</a> at least one email.
    </h2>
    <p>
Email verification helps our support team verify ownership if you lose account access and allows you to receive all the notifications you ask for.
    </p>


















</div>
</div>


      <div id="start-of-content" class="accessibility-aid"></div>
          <div class="site" itemscope itemtype="http://schema.org/WebPage">
    <div id="js-flash-container">
      
    </div>
    <div class="pagehead repohead instapaper_ignore readability-menu">
      <div class="container">
        
<ul class="pagehead-actions">

    <li class="subscription">
      <form accept-charset="UTF-8" action="/notifications/subscribe" class="js-social-container" data-autosubmit="true" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="nkpXSHnEF9lmrkjzDOEZ8No2uuZ+H0DmDpGyMlSNMZqax246+L0nuTxarHRU/UxMpfEquNkNPuRWxDyefz7XMg==" /></div>  <input id="repository_id" name="repository_id" type="hidden" value="19219512" />

    <div class="select-menu js-menu-container js-select-menu">
      <a class="social-count js-social-count" href="/bpoweski/coursera-tidy-data/watchers">
        1
      </a>
      <a href="/bpoweski/coursera-tidy-data/subscription"
        class="minibutton select-menu-button with-count js-menu-target" role="button" tabindex="0" aria-haspopup="true">
        <span class="js-select-button">
          <span class="octicon octicon-eye"></span>
          Watch
        </span>
      </a>

      <div class="select-menu-modal-holder">
        <div class="select-menu-modal subscription-menu-modal js-menu-content" aria-hidden="true">
          <div class="select-menu-header">
            <span class="select-menu-title">Notifications</span>
            <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
          </div> <!-- /.select-menu-header -->

          <div class="select-menu-list js-navigation-container" role="menu">

            <div class="select-menu-item js-navigation-item selected" role="menuitem" tabindex="0">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <div class="select-menu-item-text">
                <input checked="checked" id="do_included" name="do" type="radio" value="included" />
                <h4>Not watching</h4>
                <span class="description">Be notified when participating or @mentioned.</span>
                <span class="js-select-button-text hidden-select-button-text">
                  <span class="octicon octicon-eye"></span>
                  Watch
                </span>
              </div>
            </div> <!-- /.select-menu-item -->

            <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
              <span class="select-menu-item-icon octicon octicon octicon-check"></span>
              <div class="select-menu-item-text">
                <input id="do_subscribed" name="do" type="radio" value="subscribed" />
                <h4>Watching</h4>
                <span class="description">Be notified of all conversations.</span>
                <span class="js-select-button-text hidden-select-button-text">
                  <span class="octicon octicon-eye"></span>
                  Unwatch
                </span>
              </div>
            </div> <!-- /.select-menu-item -->

            <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <div class="select-menu-item-text">
                <input id="do_ignore" name="do" type="radio" value="ignore" />
                <h4>Ignoring</h4>
                <span class="description">Never be notified.</span>
                <span class="js-select-button-text hidden-select-button-text">
                  <span class="octicon octicon-mute"></span>
                  Stop ignoring
                </span>
              </div>
            </div> <!-- /.select-menu-item -->

          </div> <!-- /.select-menu-list -->

        </div> <!-- /.select-menu-modal -->
      </div> <!-- /.select-menu-modal-holder -->
    </div> <!-- /.select-menu -->

</form>
    </li>

  <li>
    
  <div class="js-toggler-container js-social-container starring-container ">

    <form accept-charset="UTF-8" action="/bpoweski/coursera-tidy-data/unstar" class="js-toggler-form starred js-unstar-button" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="5QMEI3TQtwi8BLXn8xSN/MZaONLNQBAbNo5zoWs7O1I8VizkCZYRDGFa+4vsUIhiZJvm4xToqnk96LqehYJmmg==" /></div>
      <button
        class="minibutton with-count js-toggler-target star-button"
        aria-label="Unstar this repository" title="Unstar bpoweski/coursera-tidy-data">
        <span class="octicon octicon-star"></span>
        Unstar
      </button>
        <a class="social-count js-social-count" href="/bpoweski/coursera-tidy-data/stargazers">
          0
        </a>
</form>
    <form accept-charset="UTF-8" action="/bpoweski/coursera-tidy-data/star" class="js-toggler-form unstarred js-star-button" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="2l5RI8qCwC0heCIFd+YTbJmNNYzP5uvMoGlJB90vAArUiYtvpm9MXNldqdvsXe/2M4Elw0xgZ6PTObbPFTk51Q==" /></div>
      <button
        class="minibutton with-count js-toggler-target star-button"
        aria-label="Star this repository" title="Star bpoweski/coursera-tidy-data">
        <span class="octicon octicon-star"></span>
        Star
      </button>
        <a class="social-count js-social-count" href="/bpoweski/coursera-tidy-data/stargazers">
          0
        </a>
</form>  </div>

  </li>


        <li>
          <a href="/bpoweski/coursera-tidy-data/fork" class="minibutton with-count js-toggler-target fork-button tooltipped-n" title="Fork your own copy of bpoweski/coursera-tidy-data to your account" aria-label="Fork your own copy of bpoweski/coursera-tidy-data to your account" rel="nofollow" data-method="post">
            <span class="octicon octicon-repo-forked"></span>
            Fork
          </a>
          <a href="/bpoweski/coursera-tidy-data/network" class="social-count">8</a>
        </li>

</ul>

        <h1 itemscope itemtype="http://data-vocabulary.org/Breadcrumb" class="entry-title public">
          <span class="mega-octicon octicon-repo"></span>
          <span class="author"><a href="/bpoweski" class="url fn" itemprop="url" rel="author"><span itemprop="title">bpoweski</span></a></span><!--
       --><span class="path-divider">/</span><!--
       --><strong><a href="/bpoweski/coursera-tidy-data" class="js-current-repository" data-pjax="#js-repo-pjax-container">coursera-tidy-data</a></strong>

          <span class="page-context-loader">
            <img alt="" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
          </span>

        </h1>
      </div><!-- /.container -->
    </div><!-- /.repohead -->

    <div class="container">
      <div class="repository-with-sidebar repo-container new-discussion-timeline  ">
        <div class="repository-sidebar clearfix">
            
<nav class="sunken-menu repo-nav js-repo-nav js-sidenav-container-pjax js-octicon-loaders"
     role="navigation"
     data-pjax="#js-repo-pjax-container"
     data-issue-count-url="/bpoweski/coursera-tidy-data/issues/counts">
  <ul class="sunken-menu-group">
    <li class="tooltipped tooltipped-w" aria-label="Code">
      <a href="/bpoweski/coursera-tidy-data" aria-label="Code" class="selected js-selected-navigation-item sunken-menu-item" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /bpoweski/coursera-tidy-data">
        <span class="octicon octicon-code"></span> <span class="full-word">Code</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>

      <li class="tooltipped tooltipped-w" aria-label="Issues">
        <a href="/bpoweski/coursera-tidy-data/issues" aria-label="Issues" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /bpoweski/coursera-tidy-data/issues">
          <span class="octicon octicon-issue-opened"></span> <span class="full-word">Issues</span>
          <span class="js-issue-replace-counter"></span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>

    <li class="tooltipped tooltipped-w" aria-label="Pull Requests">
      <a href="/bpoweski/coursera-tidy-data/pulls" aria-label="Pull Requests" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g p" data-selected-links="repo_pulls /bpoweski/coursera-tidy-data/pulls">
          <span class="octicon octicon-git-pull-request"></span> <span class="full-word">Pull Requests</span>
          <span class="js-pull-replace-counter"></span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>


      <li class="tooltipped tooltipped-w" aria-label="Wiki">
        <a href="/bpoweski/coursera-tidy-data/wiki" aria-label="Wiki" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g w" data-selected-links="repo_wiki /bpoweski/coursera-tidy-data/wiki">
          <span class="octicon octicon-book"></span> <span class="full-word">Wiki</span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>
  </ul>
  <div class="sunken-menu-separator"></div>
  <ul class="sunken-menu-group">

    <li class="tooltipped tooltipped-w" aria-label="Pulse">
      <a href="/bpoweski/coursera-tidy-data/pulse" aria-label="Pulse" class="js-selected-navigation-item sunken-menu-item" data-selected-links="pulse /bpoweski/coursera-tidy-data/pulse">
        <span class="octicon octicon-pulse"></span> <span class="full-word">Pulse</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>

    <li class="tooltipped tooltipped-w" aria-label="Graphs">
      <a href="/bpoweski/coursera-tidy-data/graphs" aria-label="Graphs" class="js-selected-navigation-item sunken-menu-item" data-selected-links="repo_graphs repo_contributors /bpoweski/coursera-tidy-data/graphs">
        <span class="octicon octicon-graph"></span> <span class="full-word">Graphs</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>
  </ul>


</nav>

              <div class="only-with-full-nav">
                
  
<div class="clone-url open"
  data-protocol-type="http"
  data-url="/users/set_protocol?protocol_selector=http&amp;protocol_type=clone">
  <h3><span class="text-emphasized">HTTPS</span> clone URL</h3>
  <div class="input-group js-zeroclipboard-container">
    <input type="text" class="input-mini input-monospace js-url-field js-zeroclipboard-target"
           value="https://github.com/bpoweski/coursera-tidy-data.git" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>

  
<div class="clone-url "
  data-protocol-type="ssh"
  data-url="/users/set_protocol?protocol_selector=ssh&amp;protocol_type=clone">
  <h3><span class="text-emphasized">SSH</span> clone URL</h3>
  <div class="input-group js-zeroclipboard-container">
    <input type="text" class="input-mini input-monospace js-url-field js-zeroclipboard-target"
           value="git@github.com:bpoweski/coursera-tidy-data.git" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>

  
<div class="clone-url "
  data-protocol-type="subversion"
  data-url="/users/set_protocol?protocol_selector=subversion&amp;protocol_type=clone">
  <h3><span class="text-emphasized">Subversion</span> checkout URL</h3>
  <div class="input-group js-zeroclipboard-container">
    <input type="text" class="input-mini input-monospace js-url-field js-zeroclipboard-target"
           value="https://github.com/bpoweski/coursera-tidy-data" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>



<p class="clone-options">You can clone with
  <a href="#" class="js-clone-selector" data-protocol="http">HTTPS</a>, <a href="#" class="js-clone-selector" data-protocol="ssh">SSH</a>, or <a href="#" class="js-clone-selector" data-protocol="subversion">Subversion</a>.
  <a href="https://help.github.com/articles/which-remote-url-should-i-use" class="help tooltipped tooltipped-n" aria-label="Get help on which URL is right for you.">
    <span class="octicon octicon-question"></span>
  </a>
</p>


  <a href="github-windows://openRepo/https://github.com/bpoweski/coursera-tidy-data" class="minibutton sidebar-button" title="Save bpoweski/coursera-tidy-data to your computer and use it in GitHub Desktop." aria-label="Save bpoweski/coursera-tidy-data to your computer and use it in GitHub Desktop.">
    <span class="octicon octicon-device-desktop"></span>
    Clone in Desktop
  </a>

                <a href="/bpoweski/coursera-tidy-data/archive/master.zip"
                   class="minibutton sidebar-button"
                   aria-label="Download the contents of bpoweski/coursera-tidy-data as a zip file"
                   title="Download the contents of bpoweski/coursera-tidy-data as a zip file"
                   rel="nofollow">
                  <span class="octicon octicon-cloud-download"></span>
                  Download ZIP
                </a>
              </div>
        </div><!-- /.repository-sidebar -->

        <div id="js-repo-pjax-container" class="repository-content context-loader-container" data-pjax-container>
          

<a href="/bpoweski/coursera-tidy-data/blob/142fe06ac8722571c66ea30ed55a5a929603d5fc/CodeBook.md" class="hidden js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:2ba0c89c87c657411be055503f54dc7e -->

<div class="file-navigation js-zeroclipboard-container">
  
<div class="select-menu js-menu-container js-select-menu left">
  <span class="minibutton select-menu-button js-menu-target css-truncate" data-hotkey="w"
    data-master-branch="master"
    data-ref="master"
    title="master"
    role="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
    <span class="octicon octicon-git-branch"></span>
    <i>branch:</i>
    <span class="js-select-button css-truncate-target">master</span>
  </span>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax aria-hidden="true">

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <span class="select-menu-title">Switch branches/tags</span>
        <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
      </div> <!-- /.select-menu-header -->

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Filter branches/tags" id="context-commitish-filter-field" class="js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
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

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <div class="select-menu-item js-navigation-item selected">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <a href="/bpoweski/coursera-tidy-data/blob/master/CodeBook.md"
                 data-name="master"
                 data-skip-pjax="true"
                 rel="nofollow"
                 class="js-navigation-open select-menu-item-text css-truncate-target"
                 title="master">master</a>
            </div> <!-- /.select-menu-item -->
        </div>

          <div class="select-menu-no-results">Nothing to show</div>
      </div> <!-- /.select-menu-list -->

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div> <!-- /.select-menu-list -->

    </div> <!-- /.select-menu-modal -->
  </div> <!-- /.select-menu-modal-holder -->
</div> <!-- /.select-menu -->

  <div class="button-group right">
    <a href="/bpoweski/coursera-tidy-data/find/master"
          class="js-show-file-finder minibutton empty-icon tooltipped tooltipped-s"
          data-pjax
          data-hotkey="t"
          aria-label="Quickly jump between files">
      <span class="octicon octicon-list-unordered"></span>
    </a>
    <button aria-label="Copy file path to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
  </div>

  <div class="breadcrumb js-zeroclipboard-target">
    <span class='repo-root js-repo-root'><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/bpoweski/coursera-tidy-data" class="" data-branch="master" data-direction="back" data-pjax="true" itemscope="url"><span itemprop="title">coursera-tidy-data</span></a></span></span><span class="separator">/</span><strong class="final-path">CodeBook.md</strong>
  </div>
</div>


  <div class="commit file-history-tease">
    <div class="file-history-tease-header">
        <img alt="Ben Poweski" class="avatar" data-user="103650" height="24" src="https://avatars2.githubusercontent.com/u/103650?v=3&amp;s=48" width="24" />
        <span class="author"><a href="/bpoweski" rel="author">bpoweski</a></span>
        <time datetime="2014-04-27T22:30:08Z" is="relative-time">Apr 27, 2014</time>
        <div class="commit-title">
            <a href="/bpoweski/coursera-tidy-data/commit/1f8d9feb571a6326d901ae95b129c2d930f1b795" class="message" data-pjax="true" title="Update CodeBook.md">Update CodeBook.md</a>
        </div>
    </div>

    <div class="participation">
      <p class="quickstat">
        <a href="#blob_contributors_box" rel="facebox">
          <strong>1</strong>
           contributor
        </a>
      </p>
      
    </div>
    <div id="blob_contributors_box" style="display:none">
      <h2 class="facebox-header">Users who have contributed to this file</h2>
      <ul class="facebox-user-list">
          <li class="facebox-user-list-item">
            <img alt="Ben Poweski" data-user="103650" height="24" src="https://avatars2.githubusercontent.com/u/103650?v=3&amp;s=48" width="24" />
            <a href="/bpoweski">bpoweski</a>
          </li>
      </ul>
    </div>
  </div>

<div class="file-box">
  <div class="file">
    <div class="meta clearfix">
      <div class="info file-name">
          <span>93 lines (83 sloc)</span>
          <span class="meta-divider"></span>
        <span>5.485 kb</span>
      </div>
      <div class="actions">
        <div class="button-group">
          <a href="/bpoweski/coursera-tidy-data/raw/master/CodeBook.md" class="minibutton " id="raw-url">Raw</a>
            <a href="/bpoweski/coursera-tidy-data/blame/master/CodeBook.md" class="minibutton js-update-url-with-hash">Blame</a>
          <a href="/bpoweski/coursera-tidy-data/commits/master/CodeBook.md" class="minibutton " rel="nofollow">History</a>
        </div><!-- /.button-group -->

          <a class="octicon-button tooltipped tooltipped-nw"
             href="github-windows://openRepo/https://github.com/bpoweski/coursera-tidy-data?branch=master&amp;filepath=CodeBook.md" aria-label="Open this file in GitHub for Windows">
              <span class="octicon octicon-device-desktop"></span>
          </a>

              <a class="octicon-button tooltipped tooltipped-n js-update-url-with-hash"
                 aria-label="Clicking this button will fork this project so you can edit the file"
                 href="/bpoweski/coursera-tidy-data/edit/master/CodeBook.md"
                 data-method="post" rel="nofollow"><span class="octicon octicon-pencil"></span></a>

            <a class="octicon-button danger tooltipped tooltipped-s"
               href="/bpoweski/coursera-tidy-data/delete/master/CodeBook.md"
               aria-label="Fork this project and delete file"
               data-method="post" data-test-id="delete-blob-file" rel="nofollow">
          <span class="octicon octicon-trashcan"></span>
        </a>
      </div><!-- /.actions -->
    </div>
    
  <div id="readme" class="blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="mainContentOfPage"><h2>
<a id="user-content-code-book" class="anchor" href="#code-book" aria-hidden="true"><span class="octicon octicon-link"></span></a>Code Book</h2>

<p>For the provided UCI HAR Dataset the following vars are set from run_analysis.R.  See the <a href="/bpoweski/coursera-tidy-data/blob/master/README.md">README</a> for additional details.</p>

<h3>
<a id="user-content-tidy-mean" class="anchor" href="#tidy-mean" aria-hidden="true"><span class="octicon octicon-link"></span></a>Tidy Mean</h3>

<p>A data.table named <code>tidy.mean</code> is set with the following columns.  All units are maintained from the original data set. A file named tidy.mean.txt is written from run_analysis.R.</p>

<table>
<thead>
<tr>
<th>column</th>
<th>description</th>
<th>type</th>
</tr>
</thead>
<tbody>
<tr>
<td>Subject</td>
<td>Identifier of the subject</td>
<td>integer</td>
</tr>
<tr>
<td>Activity</td>
<td>Label of the activity</td>
<td>factor</td>
</tr>
<tr>
<td>MeanSamples</td>
<td>Mean of variables by Subject + Activity provided in tidy</td>
<td>numeric</td>
</tr>
</tbody>
</table>

<h3>
<a id="user-content-tidy" class="anchor" href="#tidy" aria-hidden="true"><span class="octicon octicon-link"></span></a>Tidy</h3>

<p>A data.table named <code>tidy</code> is set with the following columns.  All units are maintained from the original data set. A file named tidy.txt is written from run_analysis.R.</p>

<table>
<thead>
<tr>
<th>Column</th>
<th>Original Name</th>
</tr>
</thead>
<tbody>
<tr>
<td>Activity</td>
<td></td>
</tr>
<tr>
<td>Subject</td>
<td></td>
</tr>
<tr>
<td>Time.BodyAcc.Mean.X</td>
<td>tBodyAcc-mean()-X</td>
</tr>
<tr>
<td>Time.BodyAcc.Mean.Y</td>
<td>tBodyAcc-mean()-Y</td>
</tr>
<tr>
<td>Time.BodyAcc.Mean.Z</td>
<td>tBodyAcc-mean()-Z</td>
</tr>
<tr>
<td>Time.BodyAcc.Std.X</td>
<td>tBodyAcc-std()-X</td>
</tr>
<tr>
<td>Time.BodyAcc.Std.Y</td>
<td>tBodyAcc-std()-Y</td>
</tr>
<tr>
<td>Time.BodyAcc.Std.Z</td>
<td>tBodyAcc-std()-Z</td>
</tr>
<tr>
<td>Time.GravityAcc.Mean.X</td>
<td>tGravityAcc-mean()-X</td>
</tr>
<tr>
<td>Time.GravityAcc.Mean.Y</td>
<td>tGravityAcc-mean()-Y</td>
</tr>
<tr>
<td>Time.GravityAcc.Mean.Z</td>
<td>tGravityAcc-mean()-Z</td>
</tr>
<tr>
<td>Time.GravityAcc.Std.X</td>
<td>tGravityAcc-std()-X</td>
</tr>
<tr>
<td>Time.GravityAcc.Std.Y</td>
<td>tGravityAcc-std()-Y</td>
</tr>
<tr>
<td>Time.GravityAcc.Std.Z</td>
<td>tGravityAcc-std()-Z</td>
</tr>
<tr>
<td>Time.BodyAccJerk.Mean.X</td>
<td>tBodyAccJerk-mean()-X</td>
</tr>
<tr>
<td>Time.BodyAccJerk.Mean.Y</td>
<td>tBodyAccJerk-mean()-Y</td>
</tr>
<tr>
<td>Time.BodyAccJerk.Mean.Z</td>
<td>tBodyAccJerk-mean()-Z</td>
</tr>
<tr>
<td>Time.BodyAccJerk.Std.X</td>
<td>tBodyAccJerk-std()-X</td>
</tr>
<tr>
<td>Time.BodyAccJerk.Std.Y</td>
<td>tBodyAccJerk-std()-Y</td>
</tr>
<tr>
<td>Time.BodyAccJerk.Std.Z</td>
<td>tBodyAccJerk-std()-Z</td>
</tr>
<tr>
<td>Time.BodyGyro.Mean.X</td>
<td>tBodyGyro-mean()-X</td>
</tr>
<tr>
<td>Time.BodyGyro.Mean.Y</td>
<td>tBodyGyro-mean()-Y</td>
</tr>
<tr>
<td>Time.BodyGyro.Mean.Z</td>
<td>tBodyGyro-mean()-Z</td>
</tr>
<tr>
<td>Time.BodyGyro.Std.X</td>
<td>tBodyGyro-std()-X</td>
</tr>
<tr>
<td>Time.BodyGyro.Std.Y</td>
<td>tBodyGyro-std()-Y</td>
</tr>
<tr>
<td>Time.BodyGyro.Std.Z</td>
<td>tBodyGyro-std()-Z</td>
</tr>
<tr>
<td>Time.BodyGyroJerk.Mean.X</td>
<td>tBodyGyroJerk-mean()-X</td>
</tr>
<tr>
<td>Time.BodyGyroJerk.Mean.Y</td>
<td>tBodyGyroJerk-mean()-Y</td>
</tr>
<tr>
<td>Time.BodyGyroJerk.Mean.Z</td>
<td>tBodyGyroJerk-mean()-Z</td>
</tr>
<tr>
<td>Time.BodyGyroJerk.Std.X</td>
<td>tBodyGyroJerk-std()-X</td>
</tr>
<tr>
<td>Time.BodyGyroJerk.Std.Y</td>
<td>tBodyGyroJerk-std()-Y</td>
</tr>
<tr>
<td>Time.BodyGyroJerk.Std.Z</td>
<td>tBodyGyroJerk-std()-Z</td>
</tr>
<tr>
<td>Time.BodyAccMag.Mean</td>
<td>tBodyAccMag-mean()</td>
</tr>
<tr>
<td>Time.BodyAccMag.Std</td>
<td>tBodyAccMag-std()</td>
</tr>
<tr>
<td>Time.GravityAccMag.Mean</td>
<td>tGravityAccMag-mean()</td>
</tr>
<tr>
<td>Time.GravityAccMag.Std</td>
<td>tGravityAccMag-std()</td>
</tr>
<tr>
<td>Time.BodyAccJerkMag.Mean</td>
<td>tBodyAccJerkMag-mean()</td>
</tr>
<tr>
<td>Time.BodyAccJerkMag.Std</td>
<td>tBodyAccJerkMag-std()</td>
</tr>
<tr>
<td>Time.BodyGyroMag.Mean</td>
<td>tBodyGyroMag-mean()</td>
</tr>
<tr>
<td>Time.BodyGyroMag.Std</td>
<td>tBodyGyroMag-std()</td>
</tr>
<tr>
<td>Time.BodyGyroJerkMag.Mean</td>
<td>tBodyGyroJerkMag-mean()</td>
</tr>
<tr>
<td>Time.BodyGyroJerkMag.Std</td>
<td>tBodyGyroJerkMag-std()</td>
</tr>
<tr>
<td>FFT.BodyAcc.Mean.X</td>
<td>fBodyAcc-mean()-X</td>
</tr>
<tr>
<td>FFT.BodyAcc.Mean.Y</td>
<td>fBodyAcc-mean()-Y</td>
</tr>
<tr>
<td>FFT.BodyAcc.Mean.Z</td>
<td>fBodyAcc-mean()-Z</td>
</tr>
<tr>
<td>FFT.BodyAcc.Std.X</td>
<td>fBodyAcc-std()-X</td>
</tr>
<tr>
<td>FFT.BodyAcc.Std.Y</td>
<td>fBodyAcc-std()-Y</td>
</tr>
<tr>
<td>FFT.BodyAcc.Std.Z</td>
<td>fBodyAcc-std()-Z</td>
</tr>
<tr>
<td>FFT.BodyAccJerk.Mean.X</td>
<td>fBodyAccJerk-mean()-X</td>
</tr>
<tr>
<td>FFT.BodyAccJerk.Mean.Y</td>
<td>fBodyAccJerk-mean()-Y</td>
</tr>
<tr>
<td>FFT.BodyAccJerk.Mean.Z</td>
<td>fBodyAccJerk-mean()-Z</td>
</tr>
<tr>
<td>FFT.BodyAccJerk.Std.X</td>
<td>fBodyAccJerk-std()-X</td>
</tr>
<tr>
<td>FFT.BodyAccJerk.Std.Y</td>
<td>fBodyAccJerk-std()-Y</td>
</tr>
<tr>
<td>FFT.BodyAccJerk.Std.Z</td>
<td>fBodyAccJerk-std()-Z</td>
</tr>
<tr>
<td>FFT.BodyGyro.Mean.X</td>
<td>fBodyGyro-mean()-X</td>
</tr>
<tr>
<td>FFT.BodyGyro.Mean.Y</td>
<td>fBodyGyro-mean()-Y</td>
</tr>
<tr>
<td>FFT.BodyGyro.Mean.Z</td>
<td>fBodyGyro-mean()-Z</td>
</tr>
<tr>
<td>FFT.BodyGyro.Std.X</td>
<td>fBodyGyro-std()-X</td>
</tr>
<tr>
<td>FFT.BodyGyro.Std.Y</td>
<td>fBodyGyro-std()-Y</td>
</tr>
<tr>
<td>FFT.BodyGyro.Std.Z</td>
<td>fBodyGyro-std()-Z</td>
</tr>
<tr>
<td>FFT.BodyAccMag.Mean</td>
<td>fBodyAccMag-mean()</td>
</tr>
<tr>
<td>FFT.BodyAccMag.Std</td>
<td>fBodyAccMag-std()</td>
</tr>
<tr>
<td>FFT.BodyBodyAccJerkMag.Mean</td>
<td>fBodyBodyAccJerkMag-mean()</td>
</tr>
<tr>
<td>FFT.BodyBodyAccJerkMag.Std</td>
<td>fBodyBodyAccJerkMag-std()</td>
</tr>
<tr>
<td>FFT.BodyBodyGyroMag.Mean</td>
<td>fBodyBodyGyroMag-mean()</td>
</tr>
<tr>
<td>FFT.BodyBodyGyroMag.Std</td>
<td>fBodyBodyGyroMag-std()</td>
</tr>
<tr>
<td>FFT.BodyBodyGyroJerkMag.Mean</td>
<td>fBodyBodyGyroJerkMag-mean()</td>
</tr>
<tr>
<td>FFT.BodyBodyGyroJerkMag.Std</td>
<td>fBodyBodyGyroJerkMag-std()</td>
</tr>
</tbody>
</table>

<h3>
<a id="user-content-notes" class="anchor" href="#notes" aria-hidden="true"><span class="octicon octicon-link"></span></a>Notes</h3>

<p>Source data is from <a href="https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip">https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip</a>.</p>
</article>
  </div>

  </div>
</div>

<a href="#jump-to-line" rel="facebox[.linejump]" data-hotkey="l" style="display:none">Jump to Line</a>
<div id="jump-to-line" style="display:none">
  <form accept-charset="UTF-8" class="js-jump-to-line-form">
    <input class="linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" autofocus>
    <button type="submit" class="button">Go</button>
  </form>
</div>

        </div>

      </div><!-- /.repo-container -->
      <div class="modal-backdrop"></div>
    </div><!-- /.container -->
  </div><!-- /.site -->


    </div><!-- /.wrapper -->

      <div class="container">
  <div class="site-footer" role="contentinfo">
    <ul class="site-footer-links right">
      <li><a href="https://status.github.com/">Status</a></li>
      <li><a href="https://developer.github.com">API</a></li>
      <li><a href="http://training.github.com">Training</a></li>
      <li><a href="http://shop.github.com">Shop</a></li>
      <li><a href="/blog">Blog</a></li>
      <li><a href="/about">About</a></li>

    </ul>

    <a href="/" aria-label="Homepage">
      <span class="mega-octicon octicon-mark-github" title="GitHub"></span>
    </a>

    <ul class="site-footer-links">
      <li>&copy; 2015 <span title="0.05675s from github-fe133-cp1-prd.iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="/site/terms">Terms</a></li>
        <li><a href="/site/privacy">Privacy</a></li>
        <li><a href="/security">Security</a></li>
        <li><a href="/contact">Contact</a></li>
    </ul>
  </div><!-- /.site-footer -->
</div><!-- /.container -->


    <div class="fullscreen-overlay js-fullscreen-overlay" id="fullscreen_overlay">
  <div class="fullscreen-container js-suggester-container">
    <div class="textarea-wrap">
      <textarea name="fullscreen-contents" id="fullscreen-contents" class="fullscreen-contents js-fullscreen-contents" placeholder=""></textarea>
      <div class="suggester-container">
        <div class="suggester fullscreen-suggester js-suggester js-navigation-container"></div>
      </div>
    </div>
  </div>
  <div class="fullscreen-sidebar">
    <a href="#" class="exit-fullscreen js-exit-fullscreen tooltipped tooltipped-w" aria-label="Exit Zen Mode">
      <span class="mega-octicon octicon-screen-normal"></span>
    </a>
    <a href="#" class="theme-switcher js-theme-switcher tooltipped tooltipped-w"
      aria-label="Switch themes">
      <span class="octicon octicon-color-mode"></span>
    </a>
  </div>
</div>



    <div id="ajax-error-message" class="flash flash-error">
      <span class="octicon octicon-alert"></span>
      <a href="#" class="octicon octicon-x flash-close js-ajax-error-dismiss" aria-label="Dismiss error"></a>
      Something went wrong with that request. Please try again.
    </div>


      <script crossorigin="anonymous" src="https://assets-cdn.github.com/assets/frameworks-af95b05cb14b7a29b0457c26b4a1d24151f4a47842c8e74bd556622f347b9d3d.js" type="text/javascript"></script>
      <script async="async" crossorigin="anonymous" src="https://assets-cdn.github.com/assets/github-2375cf3a0e93d1c4a609a11f141832798e84933a331a88b5240af5f3aade9e2d.js" type="text/javascript"></script>
      
      
  </body>
</html>

