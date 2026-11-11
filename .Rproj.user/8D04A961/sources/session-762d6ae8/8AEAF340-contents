## ---- make-figure

#Make figure showing payments by state

state_payments <- prf_data |>
  mutate(
    Total_Payment = X1st.Round.Payment + X2nd.Round.Payment
  ) |>
  group_by(State) |>
  summarise(
    Total_Payment = sum(Total_Payment, na.rm = TRUE)
  ) |>
  arrange(desc(Total_Payment))

state_payments |>
  slice_head(n = 10) |>
  ggplot(aes(
    x = reorder(State, Total_Payment),
    y = Total_Payment
  )) +
  geom_col() +
  coord_flip() +
  labs(
    title = "Top 10 States by Provider Relief Fund High-Impact Payments",
    x = "State",
    y = "Total High-Impact Payments"
  ) +
  theme_bw()