## Version 10 (https://github.com/brave/brave-core/pull/3918)
#### initial version committed

## Version 11 (https://github.com/brave/brave-core/pull/4048)
#### Table `contribution_info`
```diff
+ contribtion_id, step, retry, amount
- probi, month, year
! date -> created_at
```

#### New table `contribution_info_publishers`

## Version 12 (https://github.com/brave/brave-core/pull/4177)
#### Table `pending_contribution`
```diff
+ pending_contribution_id
```

## Version 13 (https://github.com/brave/brave-core/pull/4202)
#### Table `promotion`
```diff
+ claimed_at
```

## Version 14 (https://github.com/brave/brave-core/pull/4317)
#### Table `unblinded_token`
```diff
# Set value for all records to 0.25
```

#### Table `promotion`
```diff
# Set approximate_value for all records to be 0.25 * suggestions
```

## Version 15 (https://github.com/brave/brave-core/pull/4354)
#### Table `activity_info`
```diff
-fk_activity_info_publisher_id
```

#### Table `contribution_info_publishers`
```diff
-fk_contribution_info_publishers_contribution_id, fk_contribution_info_publishers_publisher_id
```

#### Table `contribution_queue_publishers`
```diff
-fk_contribution_queue_publishers_publisher_key, fk_contribution_queue_publishers_id
```

#### Table `media_publisher_info`
```diff
-fk_media_publisher_info_publisher_id
```

#### Table `pending_contribution`
```diff
-fk_pending_contribution_publisher_id
```

#### Table `promotion_creds`
```diff
-fk_promotion_creds_promotion_id
```

#### Table `recurring_donation`
```diff
-fk_recurring_donation_publisher_id
```

#### Table `server_publisher_amounts`
```diff
-fk_server_publisher_amounts_publisher_key
```

#### Table `server_publisher_banner`
```diff
-fk_server_publisher_banner_publisher_key
```

#### Table `server_publisher_links`
```diff
-fk_server_publisher_links_publisher_key
```

#### Table `unblinded_tokens`
```diff
-fk_unblinded_tokens_promotion_id
```

## Version 16 (https://github.com/brave/brave-core/pull/4834)
#### Table `contribution_info`
```diff
# Fixed claimed_at value, date formates were different per records
```
