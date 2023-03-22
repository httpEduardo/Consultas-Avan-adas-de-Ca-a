# Phishing Hunting Queries

Clicking on the name of the query will bring you to the file for it in this git repo.

***Or try them out right away in your M365 Security tenant:***

Click on the '🔎' hotlink to plug the query right into your Advanced Hunting Query page

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAEAJ1TyUoDQRCts-A_DIPnDOhN8CAYUHA5eZZ20pm0s3SYHg2CH--r151JjIFoGNJdXcurV0sKKSSTW3mXTgZIc_HS417iHsRS68RIQ90CcuDZSQWNlRY2B2vAa4DFEKWhR02dx2nwe4CuBLaHr0ce9XuSa2TWOI3xwNS4UzkBq2LHrkg1GWmuEpgd7gqIJnFXP4v7AroZ-RpIg3xStpBb8g84fcJZQdY4zzwZdFq1SRVUzNRDM_vRi7DF8X7kHXtgyFIzNpBLyp5cNxVOmLcDqocU8O7gN9Cz3_Fsf_VN0SI_C3uJd8tKFvTUXjlyaWAPlAKqC2CkdsdaYwXTcX7PyNDIHTDnnFhG-1fCtexBlrwy5uxY67ruHF4DviVel-zM4WqLxL0lWoHTpGmfA2_di2Nz_q1vRcLVDrWsM-xh8t9exI1xvEvYXoDW452PSG-IctyKzQym8pG2LHACcWvOOEflP5FH9m3FztT4R8X5GtRsMTvd-St8GqPZKvbncNS-6jasbrbqcIlTzJJzX165TzrdXL4BRhV_BE4EAAA&runQuery=true&timeRangeId=week) [Emails With OAuth Requests](EmailsWithOAuthRequests.kusto)
- Hunt for potential phishing emails that link to a Microsoft OAuth login
- OAuth tokens can grant the 3rd party permissions without stealing credentials (also bypasses MFA)
- Logins take place on login.windows.net or login.microsoftonline.com which is less suspicious

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA3VRy07DMBCcMxL_YHoCqQUuHEGqIEgc4AD8gImjFmgeShxe4uOZnSZpqwZZtrOjmcnsOkEOj1eskOADGQpENDjEAc64ZloOLfEUJbl5x3HcS347Vhm-hKzoUwjzvAPvmlVF3FNtuDE9PQzLcNp5OnxSaX4O30Ra6hz1ZZetYLVOYpn6bL_SWYZa3k9KFlTfcpv6ZsfjCJc8J_-kmMjZXBsmyKWrqfyR-yPPlFXF3U_JyS9I3wo7HuElw4Tn5AalbbhOqH1hv-PJd7lTsVry3-Qfhcx5R812ObzL9ZDFGA9EI6dU0ukd952bx4Jfd_Sfbv39mRlz9Wpd9VWjP9is-ulsz3x8KlfcFzgfFJV66pPPpLVE647HXfY73ryOaePe9Db5g3Kn-ANEfysd3AIAAA&timeRangeId=week) [Mass Incoming Email](MassIncomingEmail.kusto)
- Looks for inbound emails with >50 recipients, which may indicate a mass phishing attack
- Exclude your domain from sender address for less false positives

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAEAI1UW2sTQRQ-z4L_YRqEbGCrPvhaMDQpFRqQtOKDiGyyW7M2m43ZabXij_ebb2b2llkJwy5nzpzLd65zKSSRXLYylyfJZCdaKnkpL-SvKPklG_AO-JTcgTZUAok7eZY96Ar8HDpKIhnLR0jk4G1Ax-CNZQHpLawk1BzLJGh5XmOYyhrWcylp86xlewnJPSQSSBgdg0LztoG2xe293vKegtawpOSnPBJBQilj8xQsM_wNr43oAkfJSD7gtgLvkX5GQUuX1LmHbko8BvcNPpPlLd7XfNf0tmMmR3IN-jtsWItvcJSc8yj5zOxqapss6_rNyHn5PgqfC3O_wlcivinuKd8r-j0LYnkvD6BLWFtB8p28plSBF4VjsWXyGzoFK5M5z12Mx3HMXW2G41F1RCaaClkuWJUD5P7QzxVrY3SaeinWpmAEETo0Z19UjMognLA7btg52YBugniGdS9dxbWTX9f3yEks2S85NPJ6lhrbD-B9q6ONAtLtSWjXaAILK8ycz6bP0yf2Vcn8ZA7ZjlUx1Nb1up8Dw99zClLe7PQYqsmDrb-mlJ80P0s2Kwq27vFPXeWe2FvPLS_e7uEovn7HKnfM_Tjr4YwO5Sh2vWXnq-R-and_v-svetOxcFbDUxJ38N6i7iv54bZD9629J62X8Obsai35XtV7RrkqHphNDV_2LcL8vcIsNrv2i7yVr-Ca-GfQ0p2dtSBnAzplH3W9XtPr_7dDP0-n5GfW6432Xu9KTgN73HsNvTUz6PfDnnh8Lc6JqMTfou1mPw7U7pQsxL0KDc16s7MMAu2mdmjr_AO6LBDpfAcAAA&runQuery=true&timeRangeId=week) [Phish Delivered](PhishDelivered.kusto)
- Detects high-confidence phishing or malware emails that were delivered to one or more mailboxes

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA7VT207CQBScZxP_oeFJkho-wPRBRBMT4xUefKxlgXIppFtEjB_v7GyLBSIkJmbTdnt65pyZ6dkWWjjXCmCQoeA9577AiLsAN3hCB_fczTGoxRd8prC6ZxgysiRuyucbv0-ZveLeV25xneKEUUP8PrbD7BlivQWIeDW4LrYwMXe-qkEfV9ynSDBhFY_oMP6umCFbh1kxO2fGNeNemVXFL2avpCKXkmfeZ8x1ynulhoTvDuE52SOcq6p9ZRSKJWK9zSomwmyyDT7UMyMuQFvqnCKn70W9C3pqqa5B7HzjSL3mMW2X4pFKTRdrqjDyy3vcZpZz1Cr_jh2XYj4Shy6_PQiRlb40_tm_bUd6Ja8It4yk0hGX7g7xKO7OA8vldLqeS3XtsdtPVcvoTL1yYj_FuT4_UQ15hqYmeP3LvwtrvKr6Y6L95E707LOim9oB67m61Yk6NMFz4f86Lf4EpOw4oIJDkxTpZIX6-6_yrnrzE9bc9FvI3zFz_CRXqsMd98I9NuERJVbnstj4vKslZkay18edLqMv31ro5iyyBAAA&timeRangeId=week) [Phish Link Clickers](PhishLinkClickers.kusto)
- Input FQDN of phishing website to find who clicked on the link
- Determines email address and device name of clicker
- Determines how many times the link was clicked by each person
- Determines whether the URL was blocked when the link was clicked