# virustweets1
Here are two different files that provide the dates and IDs for searches using RTWEET package on RSTUDIO using key terms  "coronavirus", "Covid-19", "sars-cov-19" 


tweet date and ID only for github, original tweets available @ryanjgautreaux gmail.com

here is exactly what I did:
######################### RTWEET - can also be used for REST-API and not only streaming
## install rtweet from CRAN
install.packages("rtweet")
install.packages("rlang")
install.packages("pillar")

## load rtweet package
library(rtweet)
library(rlang)
library(pillar)

# authorizing
create_token(
  app = "Covid neural models", ###  <---------------- Add yours here 
  consumer_key = "your consumer key", ###  <---------------- Add yours here 
  consumer_secret = "abrahadabra", ###  <---------------- Add yours here 
  access_token = "", ###  <---------------- Add yours here 
  access_secret = "") ###  <---------------- Add yours here 


tweetscoronavirus1.df <- search_tweets(
  "coronavirus", n = 17999,  retryonratelimit = TRUE, include_rts = FALSE)
etc.
