---
layout: default
title: "Developers"
---

<div class="row" style="margin-top: 1em; margin-bottom: 1em;">
  <div class="col-sm-6 col-sm-offset-1">
    <p>
      New to wxWidgets development? Have something you want to contribute, but
      don't know how? We've written up a handy contributor guide that has the
      answers you're looking for:
    </p>
    <a href="http://wiki.wxwidgets.org/Development:_How_To_Contribute" class="btn btn-lg btn-default btn-block">
      <i class="fa fa-code-fork fa-fw"></i> Contributor Guide
    </a>
  </div>
  <div class="col-sm-4 col-sm-offset-1" style="margin: 1em 0;">
    <a href="/gsoc/">
      <img src="/gsoc/2014/logo.jpg" class="img-responsive center-block" alt="Google Summer of Code 2014">
    </a>
  </div>
</div>

<div class="row">
  <div class="col-sm-6">
    <h3>Additional Guides</h3>
    <p>
      <ul>
        <li><a href="http://trac.wxwidgets.org/wiki">Developer Wiki</a></li>
        <li><a href="/develop/code-repository/">Using Version Control</a></li>
        <li><a href="http://trac.wxwidgets.org/wiki/HowToSubmitPatches">Writing Patches</a></li>
        <li><a href="http://trac.wxwidgets.org/wiki/HowToSubmitTicket">Submitting Tickets</a></li>
        <li><a href="http://trac.wxwidgets.org/wiki/Roadmap">Development Roadmap</a></li>
        <li><a href="/develop/coding-guidelines/">Coding Guidelines</a></li>
      </ul>
    </p>
    <h3>Developer Tools</h3>
    <p>
      <ul>
        <li><a href="http://trac.wxwidgets.org/browser/">Browse SVN Online (Trac)</a></li>
        <li><a href="http://svn.wxwidgets.org/viewvc/wx/">Browse SVN Online (ViewVC)</a></li>
        <li><a href="http://docs.wxwidgets.org/trunk/">Development Manual (rebuilt daily)</a></li>
        <li><a href="http://wx.ibaku.net/changelog/">SVN Log Browser</a></li>
      </ul>
    </p>
  </div>
  <div class="col-sm-6">
    <h3>Continuous Integration</h3>
    <p><a href="https://travis-ci.org/wxWidgets/wxWidgets" target="_new">
      <img alt="Build Status" src="https://travis-ci.org/wxWidgets/wxWidgets.png?branch=master" />
    </a></p>
    <p>
      wxWidgets uses <a href="http://buildbot.net/trac" target="_new">Buildbot</a>
      for automated testing. We have a number of build slaves building both
      stable and development versions of the library in different
      configurations for many platforms, please see
      <a href="http://buildbot.tt-solutions.com/wx/" target="_new">the dashboard</a>
      for the latest build results.
    </p>
    <p>
      Also, please consider setting up your own build slave as
      <a href="http://wiki.wxwidgets.org/Development:_Buildbot#Setting_up_a_Slave" target="_new">explained here</a>
      if the platform/architecture configuration you're interested in is not
      represented yet. We are particularly interested in the slaves using
      different Windows compiler versions.
    </p>
    <p>
      Also check out our <a href="https://travis-ci.org/wxWidgets/wxWidgets" target="_new">Travis CI</a>
      profile for per-commit automated test results.
    </p>
  </div>
</div>