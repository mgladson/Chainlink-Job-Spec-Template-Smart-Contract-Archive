### Optional Fields Within Direct Request Job-Specs:

(0) To explicitly set the network of the job-spec:

```evmChainID = 1```

Note: Find the list of `evmChainID` compatible with a Chainlink Node [here](https://docs.chain.link/docs/link-token-contracts/)


(1) To add the requesting smart contracts address to the job-specs whitelist:

```requesters = ["0xaaaa1F8ee20f5565510B84f9353F1E333E753B7a","0xbbbb70F0e81C6F3430dfdC9fa02fB22BdD818C4e"]```


(2) To explicitly set the minimum LINK payment of the job-spec:

1.0 LINK payment per request

```minContractPaymentLinkJuels = 1000000000000000000```

0.750 LINK payment per request

```minContractPaymentLinkJuels = 750000000000000000```

0.050 LINK payment per request

```minContractPaymentLinkJuels = 50000000000000000```


(3) To explicitly set the associated external Job-Id for the job-spec:

```externalJobID = "0EEC7E1D-D0D2-476C-A1A8-72DFB6633F02"```

Note: This is useful for updating a job-spec for a user without the need to change the job-id set within the requesting smart contract.

(4) To explicitly set a job-specific value for the equivalent global `.env` config within the chainlink node:

```minIncomingConfirmations = 1```


### References

[0] https://docs.chain.link/docs/jobs/types/direct-request/
