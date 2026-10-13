# takgon-marketplace

Claude Code 마켓플레이스 `takgon`. 플러그인 본체는 [astromelon/takgon-mods](https://github.com/astromelon/takgon-mods)에 있다.

이 저장소는 `.claude-plugin/marketplace.json` 하나만 둔다. Windows에서 파일이 많은 저장소를 `marketplace add` 하면
EPERM rename으로 실패하는 경우가 있어(takgon-mods#1) 마켓플레이스만 따로 분리했다.

```bash
claude plugin marketplace add astromelon/takgon-marketplace
claude plugin install takgon-mods@takgon
```

업데이트는 `claude plugin marketplace update takgon` → `claude plugin update takgon-mods@takgon`.
