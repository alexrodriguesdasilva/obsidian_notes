id
amount; // valor pago
paymentDate; // data do pagamento

  

@Enumerated(EnumType.STRING)

@Column(nullable = false)

private PaymentTypeEnum paymentType;

  

private String description;

}