---
title: /transaction
# position: 1.0
type: post
description: Post a new transaction.

parameters:
  - name: hash
    content: |-
      Hexadecimal string of the signed transaction.<br>
      <em>Mandatory.</em>

content_markdown: |-
  Broadcasts a signed transaction to the mainnet Electra blockchain.

left_code_blocks:
  - code_block: |-
      curl -d '{"hash":"REPLACE_BY_A_SIGNED_TRANSACTION_HEX"}' -X POST https://api.electraproject.org/transaction
    title: curl
    language: bash

right_code_blocks:
  - code_block: |2-
      {
        "message": "Transaction broadcast."
      }
    title: Response
    language: json

  - code_block: |2-
      {
        "message": "Error message."
      }
    title: Error
    language: json
---
