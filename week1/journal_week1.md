Understanding of the problem



As we want to be an app that is more trader-focused, what are different groups among current customer base (e.g., based on their trading activities, KYC profile, etc)?

- The amount of the trading money

- The frequencey of each trade and withdraw

- Segment time length

- The investment areas (symbol)



How do they differ? What are their needs?



Are there any differences/similarities amongst identified customer segments on a cohort/temporal level? Are there any insights on users moving from high value to low value segments? 

- Yes, Based on the segments and the frequency+amount of withdraw, we can tell whether they want to do investment on GoTrade.


What are the implications for the marketing strategy? 
- Different marketing strategies may have different implications on each user, for example if we push some information that the users may be interested to, they may pay more effort on this app to do more investment. So as the profit for the company may increases. On the other hands, if we juet push the same information to all the user, this may lead to negative implication.



What are the industry characteristics of my clients?



What is the goal or purpose of my model?

- Clustering the user based on the user's segments, trading history, as well the user behaviors in an approriate ways. For example, their investment interests and risk.


Who are the business users of my model and how can they use it?

- Besides the clustering mentioned above, we can recommand the product and information to each users based on the interests that we difined in the model.



What data do I have and do I understand the various fields?

```python
class user {
    
    
    deposit_id [] #deposit
    
	segment_event ['screen_name','event_tracked_at'][]
    segement_tap_event ['event_name','event_tracked_at'][]
	
    trade []
    
    withdrawal_id []
    
    churn_date [] 
    
	segment_v1 #trade level (Given by the Gotrade data)
    segment_v2 #will be generated on case study 1
}

class deposit {
    deposit_id
    deposit_value_usd
    deposit_method
    deposit_paid_at
    deposit_ranking
}

class trade {
    id		#
    symbol	# investment company name, AAPL....	
    trade_order_level_filled_at	#trading date and time
    order_type	#USD? SHARES?
    side	#buy? sell?
    qty		#the number of trade
    trade_value_usd	#trading value
    avg_price_usd	#trading value unit
}

class withdrawal {
    withdrawal_id
    withdrawal_value_usd
    withdrawal_executed_at
}
```


