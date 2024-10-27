
# WOOFi Solana Deployment contest details

- Join [Sherlock Discord](https://discord.gg/MABEWyASkp)
- Submit findings using the issue page in your private contest repo (label issues as med or high)
- [Read for more details](https://docs.sherlock.xyz/audits/watsons)

# Q&A

### Q: On what chains are the smart contracts going to be deployed?
Solana Mainnet
___

### Q: Are there any limitations on values set by admins (or other roles) in the codebase, including restrictions on array lengths?
Functions need admin authority:
claim_fee
claim_rebate_fee
create_oracle
create_pool
create_rebate_pool
deposit
set_pool_admin
set_pool_state (all handlers in this file)
set_woo_admin
set_woo_state(all handlers in this file)
___

### Q: Are there any limitations on values set by admins (or other roles) in protocols you integrate with, including restrictions on array lengths?
No.
___

### Q: For permissioned functions, please list all checks and requirements that will be made before calling the function.
No.
___

### Q: Is the codebase expected to comply with any EIPs? Can there be/are there any deviations from the specification?
No.
___

### Q: Are there any off-chain mechanisms or off-chain procedures for the protocol (keeper bots, arbitrage bots, etc.)?
We have an offchain script, posting the prices of supported tokens (sol, usdt, etc) to Wooracle contract on Solana.
___

### Q: Are there any hardcoded values that you intend to change before (some) deployments?
NO.
___

### Q: If the codebase is to be deployed on an L2, what should be the behavior of the protocol in case of sequencer issues (if applicable)? Should Sherlock assume that the Sequencer won't misbehave, including going offline?
No. Will deploy on Solana.
___

### Q: Should potential issues, like broken assumptions about function behavior, be reported if they could pose risks in future integrations, even if they might not be an issue in the context of the scope? If yes, can you elaborate on properties/invariants that should hold?
NO.
___

### Q: Please discuss any design choices you made.
N/A
___

### Q: Please list any known issues and explicitly state the acceptable risks for each known issue.
N/A
___

### Q: We will report issues where the core protocol functionality is inaccessible for at least 7 days. Would you like to override this value?
No.
___

### Q: Please provide links to previous audits (if any).
N/A
___

### Q: Please list any relevant protocol resources.
Our swap's market-making formula: https://drive.google.com/file/d/16srlNV45gnZ2zZRKQsjHG-sEMXN_ZqRc/view?usp=sharing
___

### Q: Additional audit information.
no.
___



# Audit scope


[WOOFi_Solana @ c7835fbafdb3fe154b2365fea1969058caa9ee09](https://github.com/woonetwork/WOOFi_Solana/tree/c7835fbafdb3fe154b2365fea1969058caa9ee09)
- [WOOFi_Solana/programs/rebate_manager/src/instructions/admin/add_sub_rebate.rs](WOOFi_Solana/programs/rebate_manager/src/instructions/admin/add_sub_rebate.rs)
- [WOOFi_Solana/programs/rebate_manager/src/instructions/admin/create_rebate_info.rs](WOOFi_Solana/programs/rebate_manager/src/instructions/admin/create_rebate_info.rs)
- [WOOFi_Solana/programs/rebate_manager/src/instructions/admin/create_rebate_manager.rs](WOOFi_Solana/programs/rebate_manager/src/instructions/admin/create_rebate_manager.rs)
- [WOOFi_Solana/programs/rebate_manager/src/instructions/admin/deposit_withdraw.rs](WOOFi_Solana/programs/rebate_manager/src/instructions/admin/deposit_withdraw.rs)
- [WOOFi_Solana/programs/rebate_manager/src/instructions/admin/set_admin.rs](WOOFi_Solana/programs/rebate_manager/src/instructions/admin/set_admin.rs)
- [WOOFi_Solana/programs/rebate_manager/src/instructions/claim_rebate_fee.rs](WOOFi_Solana/programs/rebate_manager/src/instructions/claim_rebate_fee.rs)
- [WOOFi_Solana/programs/rebate_manager/src/lib.rs](WOOFi_Solana/programs/rebate_manager/src/lib.rs)
- [WOOFi_Solana/programs/rebate_manager/src/state/rebate_info.rs](WOOFi_Solana/programs/rebate_manager/src/state/rebate_info.rs)
- [WOOFi_Solana/programs/rebate_manager/src/state/rebate_manager.rs](WOOFi_Solana/programs/rebate_manager/src/state/rebate_manager.rs)
- [WOOFi_Solana/programs/woofi/src/events.rs](WOOFi_Solana/programs/woofi/src/events.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/admin/claim_fee.rs](WOOFi_Solana/programs/woofi/src/instructions/admin/claim_fee.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/admin/create_config.rs](WOOFi_Solana/programs/woofi/src/instructions/admin/create_config.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/admin/create_pool.rs](WOOFi_Solana/programs/woofi/src/instructions/admin/create_pool.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/admin/create_wooracle.rs](WOOFi_Solana/programs/woofi/src/instructions/admin/create_wooracle.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/admin/deposit_withdraw.rs](WOOFi_Solana/programs/woofi/src/instructions/admin/deposit_withdraw.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/admin/incase_token_got_stuck.rs](WOOFi_Solana/programs/woofi/src/instructions/admin/incase_token_got_stuck.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/admin/pause_unpause.rs](WOOFi_Solana/programs/woofi/src/instructions/admin/pause_unpause.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/admin/set_only_admin_config.rs](WOOFi_Solana/programs/woofi/src/instructions/admin/set_only_admin_config.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/admin/set_only_owner_config.rs](WOOFi_Solana/programs/woofi/src/instructions/admin/set_only_owner_config.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/admin/set_pool_state.rs](WOOFi_Solana/programs/woofi/src/instructions/admin/set_pool_state.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/admin/set_woo_state.rs](WOOFi_Solana/programs/woofi/src/instructions/admin/set_woo_state.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/get_price.rs](WOOFi_Solana/programs/woofi/src/instructions/get_price.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/query.rs](WOOFi_Solana/programs/woofi/src/instructions/query.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/swap.rs](WOOFi_Solana/programs/woofi/src/instructions/swap.rs)
- [WOOFi_Solana/programs/woofi/src/state/mod.rs](WOOFi_Solana/programs/woofi/src/state/mod.rs)
- [WOOFi_Solana/programs/woofi/src/state/wooconfig.rs](WOOFi_Solana/programs/woofi/src/state/wooconfig.rs)
- [WOOFi_Solana/programs/woofi/src/state/woopool.rs](WOOFi_Solana/programs/woofi/src/state/woopool.rs)
- [WOOFi_Solana/programs/woofi/src/state/wooracle.rs](WOOFi_Solana/programs/woofi/src/state/wooracle.rs)
- [WOOFi_Solana/programs/woofi/src/util/decimals.rs](WOOFi_Solana/programs/woofi/src/util/decimals.rs)
- [WOOFi_Solana/programs/woofi/src/util/math.rs](WOOFi_Solana/programs/woofi/src/util/math.rs)
- [WOOFi_Solana/programs/woofi/src/util/swap_math.rs](WOOFi_Solana/programs/woofi/src/util/swap_math.rs)
- [WOOFi_Solana/programs/woofi/src/util/token.rs](WOOFi_Solana/programs/woofi/src/util/token.rs)

