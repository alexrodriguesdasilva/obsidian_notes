id

player
match_id

// Partida associada

@ManyToOne(fetch = FetchType.LAZY)

@JoinColumn(name = "match_id", nullable = false)

private MatchModel match;

  

// Exemplo de dado adicional: presença confirmada

@Column(name = "confirmed", nullable = false)

private boolean confirmed = false;

  

// Timestamp de registro

@Column(name = "joined_at")

private LocalDateTime joinedAt = LocalDateTime.now();