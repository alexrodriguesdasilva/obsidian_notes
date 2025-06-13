id

name
day_of_week
start_time
end_time
active

  

@Column(name = "created_at")

@CreationTimestamp

private LocalDateTime createdAt;

  

@Column(name = "updated_at")

@UpdateTimestamp

private LocalDateTime updatedAt;