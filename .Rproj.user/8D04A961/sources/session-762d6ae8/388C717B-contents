## ---- make-table

library(dplyr)

#Make table of top 10 recipients

top_recipients <- prf_data |>
  mutate(
    Total_Payment = X1st.Round.Payment + X2nd.Round.Payment
  ) |>
  arrange(desc(Total_Payment)) |>
  select(Name, City, State, Total_Payment) |>
  slice_head(n = 10)

knitr::kable(
  top_recipients,
  col.names = c("Hospital / Health System", "City", "State", "Total Payment"),
  caption = "Top 10 Recipients of Provider Relief Fund High-Impact Payments"
)