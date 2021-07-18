# ANA515Assignment3

<img width="394" alt="Screen Shot 2021-07-18 at 4 27 25 PM" src="https://user-images.githubusercontent.com/81721126/126082638-db86a5b2-8d8c-491e-b8a4-c73013368591.png">

The codes below were used to make the changes according to Assignment 3's rubric.

#mydata <- read_csv("downloads/StormEvents.csv")
#myvars<-c("BEGIN_DATE_TIME","END_DATEy = rename_all(x,tolower)_TIME","EPISODE_ID","EVENT_ID","STATE","STATE_FIPS","CZ_TYPE","CZ_FIPS","CZ_NAME","EVENT_TYPE","DATA_SOURCE","BEGIN_LAT","BEGIN_LON","END_LAT","END_LON")
#newdata<-mydata[myvars]
#head(newdata)
#install lubridate
#library(lubridate)
#library(tidyverse)
#newdata <- newdata%>%
 + mutate_at(vars(ends_with('_TIME')),lubridate::dmy_hms)
#head(newdata)
#library(stringr)
#newdata$STATE=str_to_title(newdata$STATE)
#head(newdata)
#newdata$CZ_NAME=str_to_title(newdata$CZ_NAME)
#head(newdata)
#newdata=filter(newdata,CZ_TYPE == "C")
#head(newdata)
#newdata %>% select(-CZ_TYPE)
#newdata$STATE_FIPS=str_pad(newdata$STATE_FIPS, width=3, side = "left", pad="0" )
#head(newdata)
#newdata$CZ_FIPS=str_pad(newdata$CZ_FIPS, width=3, side = "left", pad="0" )
#head(newdata)
#library(dplyr)
#x = unite_(newdata, "fips", c("STATE_FIPS","CZ_FIPS"))
#y = rename_all(x,tolower)
#us_state_info<-data.frame(state=state.name, region=state.region, area=state.area)
#Newset<- data.frame(table(y$state))
#newset1<-rename(newset, c("state"="Var1"))
#merged <- merge(x=newset1,y=us_state_info,by.x="state", by.y="state")
#library(ggplot2)
#storm_plot <- ggplot(merged,aes(x = area , y = Freq)) + geom_point(aes(color=region)) + labs(x="Land Area (square miles)",y = "# of storms events in 1999") 
#storm_plot

