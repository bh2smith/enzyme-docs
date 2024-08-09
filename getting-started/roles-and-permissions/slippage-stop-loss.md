# Slippage Stop-loss

This policy is designed to limit any maliciously intended (or accidental) actions which could cause a loss to the value of the vault.

It does this by limiting the value loss (i.e. slippage) that can occur via adapter actions over a “tolerance period” (a rolling 7 day period).

Vault owners can define a tolerance threshold (eg. 10%).&#x20;

Whenever an adapter action results in slippage, that slippage amount is added to a cumulative slippage total. The accumulated slippage then diminishes over the “tolerance period duration” at a constant rate based on the fund’s chosen tolerance. This policy allows bypassing the slippage checks entirely if the adapter being called is in a Council-maintained list on the AddressListRegistry (adapters that cannot be manipulated by asset managers to steal fund value).
