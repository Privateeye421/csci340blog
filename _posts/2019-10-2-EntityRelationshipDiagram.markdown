---
layout: post
title:  "Entity Relationship Diagrams"
date:   2019-10-02 22:42:11 -0500
categories: jekyll update
author: Jack Frey
---
![image]({{site.baseurl}}/assets/img/Auction_DrawIO.png)
![image]({{site.baseurl}}/assets/img/Auction_Vertabelo.png)

Breaking down the diagram by section:

The bidder section was relatively straightforward. They have a name, and an ID.
They also track to any bid submissions, and to any purchases they end up making.
They can, but do not have to, make any amount of purchases and bids that they
want.

Submissions is a way to tie together bidders and items, both of which
can have multiple attached submission, as well as bids, which can only be
one per submission.

Bids tracks time placed and amount on the bid, which are tracked here instead
of in submissions due to time and amount needing to be relatively unique, as
they are what decides who wins.

Sellers simply need their name recorded, and nothing more, Each seller must
be attached to one or more items, as you cannot be a seller if you are not
selling anything.

Item keeps track of all of the item-related information, which, due to the
nature of an auction, should be fairly unique, and can thus all be stored in the
table.

Purchases is probably the most controversial of my sections. The reason that
the information, namely money owed to auction company and purchase price, is
here instead of in sellers and bids, is in case someone is unable to pay. In
that case, tying the auction tax to a winning bet that never actually gets paid
lead to inaccurate bookkeeping. Therefore, the data gets its own table to
prevent confusion.
