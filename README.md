# to_be_cloned

library(data.table)
library(dplyr)
library(lubridate)

Output <- Input %>% filter(Date == today())

# I'm now changing things

Output <- Input %>% filter(Date >= (today() - days(1)))

Output_today <- Output %>% filter(Date == today())

# New experimental code block

Output_tomorrow <- Output %>% filter(Date > today())
