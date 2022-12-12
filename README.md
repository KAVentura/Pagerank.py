# Homework: web search with word embeddings
**Due date:**
Sunday, 11 December at midnight
## Task 1: finding similar words
```
Katherine.Ventura.24@lambda-server:~/Pagerank.py$ python3 pagerank.py --data=./data/lawfareblog.csv.gz --search_query='weapons'
```

```
INFO:root:rank=0 pagerank=0.00010651870252331719 url=www.lawfareblog.com/why-did-you-wait-moral-emptiness-and-drone-strikes
INFO:root:rank=1 pagerank=8.837293717078865e-05 url=www.lawfareblog.com/dc-district-court-dismisses-journalists-drone-lawsuit
INFO:root:rank=2 pagerank=7.521521911257878e-05 url=www.lawfareblog.com/revived-cia-drone-strike-program-comments-new-policy
INFO:root:rank=3 pagerank=7.515928155044094e-05 url=www.lawfareblog.com/us-court-appeals-dc-circuit-dismisses-suit-over-us-drone-strike
INFO:root:rank=4 pagerank=6.499315350083634e-05 url=www.lawfareblog.com/iran-shoots-down-us-drone-domestic-and-international-legal-implications
INFO:root:rank=5 pagerank=6.488132203230634e-05 url=www.lawfareblog.com/slaughterbots-and-other-anticipated-autonomous-weapons-problems
INFO:root:rank=6 pagerank=6.461629527620971e-05 url=www.lawfareblog.com/german-courts-weigh-legal-responsibility-us-drone-strikes
INFO:root:rank=7 pagerank=6.0879148804815486e-05 url=www.lawfareblog.com/shift-jsoc-drone-strikes-does-not-mean-cia-has-been-sidelined
INFO:root:rank=8 pagerank=6.054074037820101e-05 url=www.lawfareblog.com/waiving-imminent-threat-test-cia-drone-strikes-pakistan
INFO:root:rank=9 pagerank=6.030921940691769e-05 url=www.lawfareblog.com/atomwaffen-division-member-pleads-guilty-firearms-charge
```

```
Katherine.Ventura.24@lambda-server:~/Pagerank.py$ python3 pagerank2.py --data=data/lawfareblog.csv.gz --search_query='biden' --s_weight=.02
```
```
INFO:root:rank=0 pagerank=0.001851964625529945 url=www.lawfareblog.com/praise-presidents-iran-tweets
INFO:root:rank=1 pagerank=0.0017761415801942348 url=www.lawfareblog.com/executives-privilege-rethinking-presidents-power-withhold-information
INFO:root:rank=2 pagerank=0.0014753328869119287 url=www.lawfareblog.com/document-trump-revokes-obama-executive-order-counterterrorism-strike-casualty-reporting
INFO:root:rank=3 pagerank=0.0013315927935764194 url=www.lawfareblog.com/document-justice-department-inspector-general-final-report-clinton-email-investigation
INFO:root:rank=4 pagerank=0.0013214917853474617 url=www.lawfareblog.com/how-latest-trump-tower-tweet-damages-presidents-legal-defense
INFO:root:rank=5 pagerank=0.0012723174877464771 url=www.lawfareblog.com/obamas-term-end-thoughts-targeted-killing
INFO:root:rank=6 pagerank=0.0012209431733936071 url=www.lawfareblog.com/thoughts-about-obama-administrations-counterterrorism-paradigm-light-al-liby-and-ikrima-operations
INFO:root:rank=7 pagerank=0.0012017081025987864 url=www.lawfareblog.com/critique-trump-administrations-case-presidential-war-making
INFO:root:rank=8 pagerank=0.0011908655287697911 url=www.lawfareblog.com/baghdadis-death-and-presidential-speech
INFO:root:rank=9 pagerank=0.001181220868602395 url=www.lawfareblog.com/text-presidents-speech-afternoon
```

```
Katherine.Ventura.24@lambda-server:~/Pagerank.py$ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2 --personalization_vector_query='corona'
INFO:root:rank=0 pagerank=0.01936263032257557 url=www.lawfareblog.com/britains-coronavirus-response
INFO:root:rank=1 pagerank=0.01936263032257557 url=www.lawfareblog.com/prosecuting-purposeful-coronavirus-exposure-terrorism
INFO:root:rank=2 pagerank=0.017857149243354797 url=www.lawfareblog.com/rational-security-my-corona-edition
INFO:root:rank=3 pagerank=0.017857149243354797 url=www.lawfareblog.com/brexit-not-immune-coronavirus
INFO:root:rank=4 pagerank=0.01775084249675274 url=www.lawfareblog.com/chinatalk-how-party-takes-its-propaganda-global
INFO:root:rank=5 pagerank=0.017413180321455002 url=www.lawfareblog.com/lawfare-podcast-united-nations-and-coronavirus-crisis
INFO:root:rank=6 pagerank=0.01578725501894951 url=www.lawfareblog.com/paper-hearing-experts-debate-digital-contact-tracing-and-coronavirus-privacy-concerns
INFO:root:rank=7 pagerank=0.015336664393544197 url=www.lawfareblog.com/israeli-emergency-regulations-location-tracking-coronavirus-carriers
INFO:root:rank=8 pagerank=0.014914634637534618 url=www.lawfareblog.com/china-responds-coronavirus-iron-grip-information-flow
INFO:root:rank=9 pagerank=0.014065689407289028 url=www.lawfareblog.com/congressional-homeland-security-committees-seek-ways-support-state-federal-responses-coronavirus
```
