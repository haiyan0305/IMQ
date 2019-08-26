# IMQ  (interactive mentalizing questionnaire)

(reference: https://psyarxiv.com/g2zm8/  and our theory paper: https://psyarxiv.com/ftgs3/)

For different versions of  IMQ(haiyanwu3@gmail.com)

## English version 
### option 1

qualtrics and using R to calculate the scores


        #delete items 3 6  11 and  19
        IMQdata <- IMQdata %>% dplyr::mutate(IMQ_OS = IMQ_16+IMQ_12+ IMQ_1+IMQ_8+IMQ_22+IMQ_15)
        IMQdata <- IMQdata %>% dplyr::mutate(IMQ_SS = IMQ_2+IMQ_14+IMQ_17+IMQ_18+IMQ_20+IMQ_21+IMQ_24+IMQ_23)
        IMQdata <- IMQdata %>% dplyr::mutate(IMQ_SO = IMQ_9+ IMQ_7 + IMQ_4+IMQ_5+IMQ_13+IMQ_10)
        IMQdata <- IMQdata%>% dplyr::mutate(total_study1 =IMQ_OS+ IMQ_SS+IMQ_SO)



### option 2
running Eprime and get the IMQ_SS, IMQ_SO, IMO_OS and total IMQ score automatically

IMQ_EN.ebs


## Chinese version (validated by Haiyan Wu)
### option 1

wenjuanxing(wjx.com) and using R to calculate the scores

IMQ_SO: 是自我推论他人心理状态的能力
IMQ_OS: 是对于他人不能推论自己心理状态的自信
IMQ_SS: 是社会交互中心理理论的元认知（自信程度）

### option 2
running Eprime and get the IMQ_SS, IMQ_SO, IMO_OS and total IMQ score automatically

IMQ_CN.ebs


## Japanese version 
### option 1

qualtrics and using R to calculate the scores


### option 2
running Eprime and get the IMQ_SS, IMQ_SO, IMO_OS and total IMQ score automatically

IMQ_JP.ebs
