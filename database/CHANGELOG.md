## Version 10 (https://github.com/brave/brave-core/pull/3918)
#### initial version committed

## Version 11 (https://github.com/brave/brave-core/pull/4048)
#### Table `contribution_info`.
  - **Added**: `contribtion_id`, `step`, `retry`, `amount`
  - **Renamed**: `date` -> `created_at`
  - **Removed**: `probi`, `month`, `year`
  
#### New table `contribution_info_publishers` 

## Version 12 (https://github.com/brave/brave-core/pull/4177)
#### Table `pending_contribution`.
  - **Added**: `pending_contribution_id`
  
## Version 13 (https://github.com/brave/brave-core/pull/4202)
#### Table `promotion`.
  - **Added**: `claimed_at`

## Version 14 (https://github.com/brave/brave-core/pull/4317)
#### Table `unblinded_token`.
  - **Other**: Set `value` for all records to `0.25`
  
#### Table `promotion`.
  - **Other**: Set `approximate_value` for all records to be `0.25` * `suggestions`
  
## Version 15 (https://github.com/brave/brave-core/pull/4354)
#### Table `activity_info`.
  - **Removed**: `fk_activity_info_publisher_id`
  
#### Table `contribution_info_publishers`.
  - **Removed**: `fk_contribution_info_publishers_contribution_id`, `fk_contribution_info_publishers_publisher_id`
  
#### Table `contribution_queue_publishers`.
  - **Removed**: `fk_contribution_queue_publishers_publisher_key`, `fk_contribution_queue_publishers_id`
  
#### Table `media_publisher_info`.
  - **Removed**: `fk_media_publisher_info_publisher_id`
  
#### Table `pending_contribution`.
  - **Removed**: `fk_pending_contribution_publisher_id`
  
#### Table `promotion_creds`.
  - **Removed**: `fk_promotion_creds_promotion_id`
  
#### Table `recurring_donation`.
  - **Removed**: `fk_recurring_donation_publisher_id`
  
#### Table `server_publisher_amounts`.
  - **Removed**: `fk_server_publisher_amounts_publisher_key`
  
#### Table `server_publisher_banner`.
  - **Removed**: `fk_server_publisher_banner_publisher_key`
  
#### Table `server_publisher_links`.
  - **Removed**: `fk_server_publisher_links_publisher_key`
  
#### Table `unblinded_tokens`.
  - **Removed**: `fk_unblinded_tokens_promotion_id`
  
## Version 16 (https://github.com/brave/brave-core/pull/4834)
#### Table `contribution_info`.
  - **Other**: Fixed `claimed_at` value, date formates were different per records
