## Introduction ##

This section explains briefly how module is able to work and activate customer accounts using activation links. This knowledge is not required to be able to use module, I am posting this section as curio.

## Details ##

Before module can start working it needs to be added and installed, automatically or manually. During installation it registers to the hook that is executed when new account is created. Customer table is also modified and column that holds activation links for specified customer is added. Activation link is MD5 checksum of the random number so they are unique. When new account is registered hook is executed and logic from the module also is executed. This logic takes information about newly registered customer, deactivates this account and generates unique activation link for the customer. Activation link is saved to the database and mail in proper language for the customer is generated and sent. In the mail the link is written to the module front controller that will trigger activation action. The link is checked if it does meet requirement and the database is searched for the account that have activation link assigned. If no account was found that means that activation link is not valid. If one account was found that means that this account needs to be activated. Activation is being done and corresponding message is being displayed.