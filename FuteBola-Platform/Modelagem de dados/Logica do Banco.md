### 🔹 `TB_USER` → `TB_PLAYER`

**Relação:** `1:1 (obrigatória do lado do Player)`

- Um `User` pode ser um `Player`.
    
- Um `Player` **sempre** é um `User`.

### 🔹 `TB_PLAYER` → `TB_PLAYER_PAYMENT`

**Relação:** `1:N`

- Um jogador **pode ter vários pagamentos**, não apenas um.
    
- Um pagamento é **sempre** feito por um jogador.

### 🔹 `TB_PLAYER_GROUP` → `TB_PLAYER_PAYMENT`

**Relação:** `1:N (opcional no lado de Payment)`

- Um grupo pode receber **vários pagamentos**.
    
- Um pagamento pode ou não estar ligado a um grupo.

🔹 `TB_MATCH` → `TB_PLAYER_PAYMENT`
**Relação:** `1:N (opcional no lado de Payment)`

- Uma partida pode ter muitos pagamentos.
    
- Um pagamento pode estar associado a uma partida **ou não** (em caso de pagamento mensal).

🔹 `TB_PLAYER_GROUP` → `TB_MATCH`

**Relação:** `1:N (opcional)`

- Um grupo pode ter várias partidas.
    
- Uma partida pode ou não estar associada a um grupo.

### 🔹 `TB_PLAYER` ⇄ `TB_PLAYER_GROUP`

**Relação:** `N:N`  
**Tabela intermediária:** `TB_PLAYER_GROUP_MEMBER`

- Um jogador pode estar em vários grupos.
    
- Um grupo pode ter vários jogadores.