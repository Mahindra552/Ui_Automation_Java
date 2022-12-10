## Storefront UI Framework - Getting started.

Requirements:

Intelli J: [https://www.jetbrains.com/idea/download/#section=windows](https://www.jetbrains.com/idea/download/#section=windows)



Git : [https://git-scm.com/](https://git-scm.com/)

OR Sourcetree: [https://www.sourcetreeapp.com/](https://www.sourcetreeapp.com/)




For developing> create a branch off the master branch and push any changes to that branch

Then create a pull request to the master branch and once approved it can be merge.



Open your local folder to the repo in Intelli J

![](https://lh4.googleusercontent.com/_-c4uDZXbYABVZOsMNtVatLGy4uh9dP24dHynhEm16acgUtMm6FJxjU3pDDAkxBziNx8TCRCn-EDAZUSTz8UvVP5Fsfn5RaSc_FBfIMK4ySVGtVpgey37wjkv6Zis43C8XJWOQVg)



Add the pom file to the maven project by selecting the + icon

![](https://lh5.googleusercontent.com/OB0XWFmopQMdVlK5Wd0o9NVLPHsEi0h9iExsefj6tk-1MzEyyu8JlU2NDcQi2OkAVks_p1z6pAesGr8zcDA2KvBtSe6kqQVanNX1yXceJgkSbwPrtyzgee1uOOdi5v5pJA2ObnN8)



Uninstall the Substeps IntelliJ plugin




The tests are structured as follows:



-   Glue: Maps the feature file to the step definition


![](https://lh4.googleusercontent.com/DVwV5McqHVbddpR7I_kI1J3W1j4FFmQiTI-mhdBQK9_4xZ9B39up6tb1v0uNmb7EOinAUxnA32jxLz9hYVmnji-CI376fS2wfLS1Ova9mp-XWyfsBuzw6u55DWonNMnmQV8brRhd)



-   Pages: These are the elements and methods that relate to a particular page or common component




![](https://lh5.googleusercontent.com/rHc2sHkwsOvfm3NUbaz6rZIFOyyn60YVwiugeRnUhXrXQ8HU3_PrPgUPmfEfQVd3n1G2mFXhS2COuvix1hWjua022DD4puX2IqYTQQYJPS4w0zBFm0adH6VdwTRH8Au3ZAN8yLTw)



-   Steps: These are the step definitions that relate to the gherkin cucumber scenarios defined in the feature files




![](https://lh5.googleusercontent.com/HyscBooYnLGbVZ_iH72mxNMSj_g6ERFrLo5OISOdkoGeA79g0PK50Pu5OQvcb-MOTgG4QTLPlEFNC1-nlRAUPu7999lw4CzbvyLu05Wv3aAl1cHZn_iYQmHVrmBK4X0COAhFvITZ)



-   Utils: These are the classes that contain methods & interface for the Page Object Api




![](https://lh3.googleusercontent.com/CeFdNgP4ogtMO_0givpKbxCi5JhSpZqgdgAJR-om17CnTGy5XlefhAFP_j9VyRuUbjjmjn8H2_8vn76pqdBTgCxJ1a52YK5hgcZ7fBZVAh9Sp467Nkxtpa1O41C6_0_3825YkkTC)



-   Resources>features: These are the feature files that contain the highest level given-when-then scenarios




![](https://lh6.googleusercontent.com/7J0Dbc7Bw4PoQdDLQt-ogfv0uxZG9mQRw2toqxjzlHqEu7gJzXx_jK7kJ10fLO80j-dwNv3a9x2_OKKlOs0HmnhAqwtucnY5udSLQOHvclyPFnt2FlcyB6DhmjxyEpW4QV5tiURM)



## Running the test:

Execute the maven goal and specify the test and base URL. The test name is the name specified in the glue:



![](https://lh4.googleusercontent.com/76Yurfdv0EtN-9VQvdnl5wblrifpr8GBGy6eAcPBtsNxEZO6YZlx2t_PYQ-PaeHg9q4HMApZ8uR2l79WOLA--7aTF7jUNjAXS3iVv4ucek1ugnFeOiBYjLdX_43Irqm_cHiWLbHP)





Ensure that you install chrome driver to match the path as specified in the serenity properties.



![](https://lh3.googleusercontent.com/Ou6YyfAyMrQ7G-eAxsSaTcRACc74rLOwbbkCU_fCfNTkkYGRfQNufDKWjdp9JCJSsMZWrNUtyaBwG0C-E2ZEXXkzYlf1zNjMH_T0aVjEM4lJdMcWjtMgoPPCmadud4xTuczeFeU_)



Please do not change this path in serenity properties as this is the path to the chrome driver on the remote machine.



## Page Objects Api



See doc on finding PageObjects with Javascript in the browser console:

[https://confluence.buy4now.ie/display/v8/UI+Automation+with+Page+Objects+-+QA](https://confluence.buy4now.ie/display/v8/UI+Automation+with+Page+Objects+-+QA)



In Serenity these are identified using the PageObjectsApi annotation in the relevant pages class and the relevant method required from the PageObjectsApi class.



![](https://lh6.googleusercontent.com/ZEXjOK6kkzM4HRIZqo9x4mYIxjBeK9SAzmJJCj6twZmW0VTX5t-Bq48PDKAbU90c2Rhs4EKSrv0sed09rIYcEKMqOwa-VybhRLpq8rNWmA6SLh6ZrhEX9QNhQJb3-RWrvaO_0wvv)



![](https://lh5.googleusercontent.com/_Ggjs1OVtbO_M1sxubLI1m3pYSC9ftp4ZArmBOJ0r5ILK-ItVDy5uFYU5t5WxpF3OSZ7kEknRyldkcVyxXthjELtW-RYpRnYk5m0jIb_G1_eAWJssGAm-8T3nvbAbCFySAsnZDZo)