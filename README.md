# rpug-2016-11

## Puppet Ecosystem announcements
+ Puppet Puppet Agent 1.8.0 on November 1st.
  - Puppet 4.8.0 - *"This release includes several improvements to the type system and updates puppet module tool to use `forgeapi.puppet.com` (instead of `forgeapi.puppetlabs.com`)."*
  - Facter 3.5.0 - *"New feature release allowing settings for configuring external and custom fact directories, setting command line options, and blocking facts - loaded by default from `/etc/puppetlabs/facter/facter.conf`"*
+ Opensource puppet 3.x appears to be EOL on Dec 31, 2016.
+ Purely as a guess, but based on looking at the publicly available issue tracker, opensource puppet 3.x might have another bug fix release before EOL https://tickets.puppetlabs.com/browse/PUP/fixforversion/18113/?selectedTab=com.atlassian.jira.plugins.jira-development-integration-plugin:release-report-tabpanel
+ `puppetlabs-ntp` forge module has been updated to account for puppet4 style and data binding. It is supposed to be a good resource to see how to write a modern module. I would not simply just `git clone` the module or update r10k's `Puppetfile` to use the new module without first examining it and testing it.
+ Vox Pupuli is the home of a community of contributors whoworking together to ensure continued development of old or orphaned modules.
  - https://voxpupuli.org/
  - https://forge.puppet.com/puppet?utf-8=%E2%9C%93&sort=latest_release
  - And I am quite sure that zack's r10k forge module will soon fall under V.P.'s care.

## PuppetConf 2016 re-cap
+ Oooh look, someone else did a PuppetConf wrap-up
  - https://rnelson0.com/2016/10/26/puppetconf-2016-wrap-up/
+ PuppetConf videos are available today Monday Nov 7.
  - PuppetConf 2016 video playlist - https://www.youtube.com/playlist?list=PLV86BgbREluVjwwt-9UL8u2Uy8xnzpIqa
+ At the Contributor Summit, Puppet 4.7 was described as working well enough, and they don't want to disrupt puppet4.x development, so  perhaps it is time to think about releasing Puppet5.
  - Puppet5 would not be a breaking change (like 3.x to 4.x). But the language constructs and features that are `DEPRECATED` in 4.x, will certainly be removed in puppet5.
+ In a technical difficuilties break at the Contrib Summit, they did a hands raised if you are on puppet 4, puppet, 3, puppet 2.x. puppet 0.25???. The Summit is kinda preaching to the choir, and it appeared that more then half were on puppet4.

### Talks that I liked:
+ "Enjoying the Journey from Puppet 3.x to Puppet 4.x" - Rob Nelson
  - https://puppetconf2016.sched.org/event/6fj4/enjoying-the-journey-from-puppet-3x-to-4x-rob-nelson-att
  - Slides - http://www.slideshare.net/rnelson0/enjoying-the-journey-from-puppet-3x-to-puppet-4x-puppetconf-2016
  - Video - https://www.youtube.com/watch?v=FWnj0xQOZN8
  - He documents things in his talk that I experienced when I migrated from PE 3.8 to PE 2015.2.

+ "Can You Manage Me Now? Humanizing Configuration Management at Scale" – Tray Torrance, Twitter
  - https://puppetconf2016.sched.org/event/6fjK/can-you-manage-me-now-humanizing-configuration-management-at-scale-tray-torrance-twitter
  - Video - https://www.youtube.com/watch?v=0OVaz2dR9vE
  - Twitter is a huge internet property and they are on the path to consolidating from a mixed version of 2.x & 3.x down to 3.x, so that they can get to 4.x
+ "Kubernetes for Sysadmins" – Kelsey Hightower, Google
  - https://puppetconf2016.sched.org/event/6fjT/kubernetes-for-sysadmins-kelsey-hightower-google
  - Live demo that worked, and quite possibly the future of deploying services.
  - Video - https://www.youtube.com/watch?v=HlAXp0-M6SY
+ "Using HashiCorp's Vault With Puppet" – Seth Vargo, HashiCorp
  - https://puppetconf2016.sched.org/event/6fjv/using-hashicorps-vault-with-puppet-seth-vargo-hashicorp
  - Video - https://www.youtube.com/watch?v=PEdhD1hOpds
  - Puppet with good Secrets Management is something that interests many but is not solved by a single vendor. Vault and consul look to be a leader in this space.
+ "Puppet Templates" – Sally Lehman, Auth0
  - https://puppetconf2016.sched.org/event/6fjz/puppet-templates-sally-lehman-auth0
  - Video - https://www.youtube.com/watch?v=Tz6ngyPb2ew
  - Quite a comprehensive look at various forms of content templating
  - CatGIFs++
+ "How to Succeed in Relearning Puppet Without Really Trying" – Joshua Zimmerman, University of Wisconsin
  - https://puppetconf2016.sched.org/event/6fk9/how-to-succeed-in-relearning-puppet-without-really-trying-joshua-zimmerman-university-of-wisconsin
  - Video - https://www.youtube.com/watch?v=WexcudaDQY0
  - Solid look at anti-patterns in code and also biases/anti-patterns in how we learn and teach
+ "Moving from Exec to Types and Providers" – Martin Alfke, example42 GmbH
  - https://puppetconf2016.sched.org/event/6fjq/moving-from-exec-to-types-and-providers-martin-alfke-example42-gmbh
  - Video - https://www.youtube.com/watch?v=Jr8H0wSUMBY
  - Did you think writing your own Types and Providers is hard? I did too until Martin shows us how.
  - A+ talk

## Take-aways
+ Lots of desirable talks to see but I feel it was too parallelized.
+ Sponsor Keynotes were in a large 2hr block in the morning and should have been spread out.
+
+ Follow Rob Nelson's blog or his twitter account
  - He was voted Most Valuable Puppeteer 2016 at PuppetConf
  - He really does know his stuff regarding puppet code, and code testing via CI
+ The next PuppetConf is in San Francisco in Oct 2017.
