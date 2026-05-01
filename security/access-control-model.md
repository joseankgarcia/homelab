| Asset / Zone     | Access Method | Allowed Users            | Notes                               |
| ---------------- | ------------- | ------------------------ | ----------------------------------- |
| Client VLAN      | LAN only      | Internal devices         | Normal user devices                 |
| Management VLAN  | LAN / NetBird | Admin only               | Router, switch, DNS admin           |
| Services VLAN    | LAN / NetBird | Admin / approved clients | Docker services                     |
| Public Internet  | No ingress    | N/A                      | No direct public exposure           |
