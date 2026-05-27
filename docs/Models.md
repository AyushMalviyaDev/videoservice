Model Architecture Planning 

Membership model 
    -slug 
    -type (free, pro, enterprise)
    -price 
    -stripe plan id 

UserMembership 
    -user (foriegn key to default user)
    -stripe customer id 
    -membership type (foriegn key to Membership)

Subscription 
    -user membership 
    -stripe subscription id (foriegn key to UserMembership)
    -active 

Course 
    -slug
    -title 
    -description 
    -allowed membership (foriegn key to Membership)


Lesson 
    -slug 
    -title 
    -course (foriegn key to Course)
    -video 
    -thumbnail 

    