### 🔹 `TB_USER` → `TB_PLAYER`

**Relação:** `1:1 (obrigatória do lado do Player)`

- ✅ Um `User` pode ser um `Player`.
    
- ✅ Um `Player` **sempre** é um `User`.

### 🔹 `TB_PLAYER` → `TB_PLAYER_PAYMENT`

**Relação:** `1:N` (**correto seria 1:N**, não 1:1)

- ❌ Um jogador **pode ter vários pagamentos**, não apenas um.
    
- ✅ Um pagamento é **sempre** feito por um jogador.