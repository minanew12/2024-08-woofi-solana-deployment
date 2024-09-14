
# WOOFi Solana Deployment contest details

- Join [Sherlock Discord](https://discord.gg/MABEWyASkp)
- Submit findings using the issue page in your private contest repo (label issues as med or high)
- [Read for more details](https://docs.sherlock.xyz/audits/watsons)

# Q&A

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
- [WOOFi_Solana/programs/woofi/src/instructions/admin/mod.rs](WOOFi_Solana/programs/woofi/src/instructions/admin/mod.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/admin/pause_unpause.rs](WOOFi_Solana/programs/woofi/src/instructions/admin/pause_unpause.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/admin/set_only_admin_config.rs](WOOFi_Solana/programs/woofi/src/instructions/admin/set_only_admin_config.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/admin/set_only_owner_config.rs](WOOFi_Solana/programs/woofi/src/instructions/admin/set_only_owner_config.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/admin/set_pool_state.rs](WOOFi_Solana/programs/woofi/src/instructions/admin/set_pool_state.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/admin/set_woo_state.rs](WOOFi_Solana/programs/woofi/src/instructions/admin/set_woo_state.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/get_price.rs](WOOFi_Solana/programs/woofi/src/instructions/get_price.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/mod.rs](WOOFi_Solana/programs/woofi/src/instructions/mod.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/query.rs](WOOFi_Solana/programs/woofi/src/instructions/query.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/swap.rs](WOOFi_Solana/programs/woofi/src/instructions/swap.rs)
- [WOOFi_Solana/programs/woofi/src/instructions/try_query.rs](WOOFi_Solana/programs/woofi/src/instructions/try_query.rs)
- [WOOFi_Solana/programs/woofi/src/lib.rs](WOOFi_Solana/programs/woofi/src/lib.rs)
- [WOOFi_Solana/programs/woofi/src/state/mod.rs](WOOFi_Solana/programs/woofi/src/state/mod.rs)
- [WOOFi_Solana/programs/woofi/src/state/wooconfig.rs](WOOFi_Solana/programs/woofi/src/state/wooconfig.rs)
- [WOOFi_Solana/programs/woofi/src/state/woopool.rs](WOOFi_Solana/programs/woofi/src/state/woopool.rs)
- [WOOFi_Solana/programs/woofi/src/state/wooracle.rs](WOOFi_Solana/programs/woofi/src/state/wooracle.rs)
- [WOOFi_Solana/programs/woofi/src/util/decimals.rs](WOOFi_Solana/programs/woofi/src/util/decimals.rs)
- [WOOFi_Solana/programs/woofi/src/util/math.rs](WOOFi_Solana/programs/woofi/src/util/math.rs)
- [WOOFi_Solana/programs/woofi/src/util/mod.rs](WOOFi_Solana/programs/woofi/src/util/mod.rs)
- [WOOFi_Solana/programs/woofi/src/util/swap_math.rs](WOOFi_Solana/programs/woofi/src/util/swap_math.rs)
- [WOOFi_Solana/programs/woofi/src/util/token.rs](WOOFi_Solana/programs/woofi/src/util/token.rs)


