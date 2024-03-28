+++
title = 'Golang Postgres Hell'
date = 2024-03-27T21:51:14-04:00
draft = false
tags = ["nesrm","go/golang"]
categories = ["nesrm"]
projects = ["nesrm"]
+++
# This Is Harder Than It Should Be
Step to making a high frequency read write database. Make an API to reduce user facing applications from having to call stupid queries that mess stuff up. What a great chance to learn Rust or Go. I chose Go. Problem with Go is I'd argue everyone who's active in Go instead of Rust works in too loose of a way, and doesn't believe in properly documenting things, or a good youtube channel to centralize around. 
## Supabase
I initally tried using the go supabase library. Oh wait there's two both called supabase-go. And both are poorly documented. And both broke on me. After running in circles, let's go to the next option

## PostgreSQL Driver
Be a big boy, why need all the niceties that supabase provides. Just do it yourself. High speed `/pgx` right. No. For how reccomened, and how much it's pushed, why is the documentation so poor. Also my Issue still hasn't been responded to so, guess I'm shit out of luck

### Unbelievable Issue
Turns out, the parser is broken for pgx for connection strings. It doesn't parse it properly. So after a long day of figuring out how to fix it, I gave up and am now using a DSN URL. 

# End
I have finally connected to a datbase. Time to work on actually using it. Bright things ahead
