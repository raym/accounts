# @accounts/graphql-api

## 0.33.0
### Minor Changes



- [#1150](https://github.com/accounts-js/accounts/pull/1150) [`22056642`](https://github.com/accounts-js/accounts/commit/220566425755a7015569d8e518095701ff7122e2) Thanks [@larsivi](https://github.com/larsivi)! - Add support for magic-link strategy 🎉.
  
  Installation:
  
  ```sh
  yarn add @accounts/magic-link
  ```
  
  Usage:
  
  ```js
  import AccountsMagicLink from '@accounts/magic-link';
  
  const accountsMagicLink = new AccountsMagicLink({});
  
  const accountsServer = new AccountsServer(
    { db: accountsDb, tokenSecret: 'secret' },
    {
      magicLink: accountsMagicLink,
    }
  );
  ```

### Patch Changes



- [#1135](https://github.com/accounts-js/accounts/pull/1135) [`304cc18d`](https://github.com/accounts-js/accounts/commit/304cc18d84d8153b7a4e857753eea85fa9f7a1f2) Thanks [@pradel](https://github.com/pradel)! - Upgrade dependencies



- [#1137](https://github.com/accounts-js/accounts/pull/1137) [`7726eaf7`](https://github.com/accounts-js/accounts/commit/7726eaf7fb12eb848de5dab0913a12a2e0283954) Thanks [@pradel](https://github.com/pradel)! - Fix `accountsGraphQL.context` breaking apollo subscriptions.