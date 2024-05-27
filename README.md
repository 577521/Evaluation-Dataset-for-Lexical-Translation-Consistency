# Evaluation-Dataset-for-Lexical-Translation-Consistency
`Paper`: [Evaluation Dataset for Lexical Translation Consistency in Chinese-to-English Document-level Translation](https://aclanthology.org/2024.lrec-main.583/)

This paper proposes a dataset to evaluate lexical translation consistency in Chinese-to-English document-level translation.

This dataset ontains a total of 310 bilingual news articles from China Daily, with a total of 5,051 sentences, and an average of 16 sentences per article. 

#### If you use the dataset for your research, please cite:
```
@inproceedings{lei-etal-2024-evaluation-dataset,
    title = "Evaluation Dataset for Lexical Translation Consistency in {C}hinese-to-{E}nglish Document-level Translation",
    author = "Lei, Xiangyu and Li, Junhui and Tao, Shimin and Yang, Hao",
    booktitle = "Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024)",
    month = may,
    year = "2024",
    address = "Torino, Italia",
    publisher = "ELRA and ICCL",
    url = "https://aclanthology.org/2024.lrec-main.583",
    pages = "6575--6581",
}
```

#### Annotation Format
For each document, there are:
- `zh2en_raw`: the original Chinese and English document. Each line is a Chinese sentence and its English translation, separated by (` ||| `).
- `zh2en_token`: the tokenized Chinese and English document. Each line is a Chinese sentence and its English translation, separated by (` ||| `).
- `res`: All repeated source words that are annotated as should be translated consistently. Each line is a repeated source word, its corresponding Chinese sentence number, its position number within the sentence and its English translation, separated by (`/`).
#### Example
Taking the first document as an example:

`zh2en_raw/test-1.txt`:
```
一位医生计划在墨西哥湾开设一家“漂浮医疗诊所”，为有需要的女性进行堕胎手术。 ||| A doctor plans to open a floating health clinic in the Gulf of Mexico where women can get surgical abortions.
保护受州法律威胁的女性生殖权利（PRROWESS）”组织将提供生殖健康和保健服务，包括避孕和怀孕14周内的流产手术。 ||| PRROWESS, which stands for Protecting Reproductive Rights of Women Endangered by State Statutes, will offer reproductive health and wellness services, including contraception as well as surgical abortion up to 14 weeks.
据PRROWESS网站介绍，漂浮诊所主要为居住在德克萨斯州、路易斯安那州和墨西哥湾沿岸其他州的患者提供服务，目标是每月营业三周左右。 ||| The clinic will serve patients who live primarily in Texas, Louisiana and other states located on the Gulf Coast, with a goal of operating for approximately three weeks out of each month, according to the organization's website.
该组织表示：“漂浮诊所将接受海岸警卫队的检查，并设置直升机通道，用于运输和紧急情况。” ||| "The vessel will be Coast Guard inspected and will have helicopter access for transport and emergencies," the organization says.
此类设施已被军方和救援组织使用多年，该组织表示，调查表明，患者愿意在漂浮诊所接受治疗。 ||| These types of facilities have been used by the military and relief organizations for years and the organization says research shows patients are willing to seek care in a floating clinic.
漂浮诊所将在联邦水域内运营，因此其活动不受州法律限制。 ||| The clinic will operate in federal waters so its activities will not be restricted by state laws.
上个月，美国联邦最高法院推翻了罗伊诉韦德案，这意味着许多州现在可以限制或禁止堕胎。 ||| The Supreme Court overturned Roe v. Wade last month, meaning many states can now restrict or ban access to abortions.
由于在墨西哥湾沿岸地区人们往往很难获得医疗服务，而且并非所有患者都可以选择前往其他州，PRROWESS旨在为这些人提供更便捷的服务。 ||| Because it is often difficult for people to access care in Gulf states and flying out of state might not be an option for all patients, PRROWESS aims to offer faster services for those people.
该组织表示，对患者进行术前检查后，将安排将其送往漂浮诊所。 ||| Once a patient is pre-screened, arrangements will be made to transport them to the floating clinic, the organization says.
加州大学旧金山分校的梅格·奥特里博士告诉哥伦比亚广播公司旧金山频道：“人们对自己身体有自主权和选择权，所以有权怀孕，也有权不怀孕。” ||| "This is all about bodily autonomy and choice, and so people have a right to be pregnant and also not to have a pregnancy," Dr. Meg Autry, of the University of California—San Francisco, told CBS San Francisco.
奥特里是加州大学旧金山分校妇产科和生殖科学系研究生医学教育和继续医学教育副主席，她希望以低费用或免费的方式提供服务。 ||| Autry, who is vice chair of graduate medical education and continuing medical education for the Department of Obstetrics, Gynecology and Reproductive Sciences at UCSF, wants to offer the services at low or no cost.
然而，据估计漂浮诊所成本至少2000万美元，PRROWESS正在寻求捐款，包括捐赠一艘船。 ||| The vessel, however, is expected to cost at least $20 million, and the organization is looking for donations, including a donated boat.
奥特里希望在一年内开设这家漂浮诊所，但她清楚这么做的挑战。 ||| She hopes to open the floating clinic in about a year, but knows there will be challenges.
她说：“这涉及到运营、物流、海事法，当然还有安全、责任，我的意思是面前有无数挑战。” ||| "There's operational, logistics, there's the whole idea of maritime law and then there's obviously security, there's liability, I mean the challenges are countless," Autry said.
包括得克萨斯州和路易斯安那州在内的13个州都颁布了所谓的“触发法”，在罗诉韦德案裁决被推翻后限制堕胎，而其他州将在30天内生效。 ||| Thirteen states, including Texas and Louisiana have so-called "trigger" laws that would restrict abortion with Roe overturned, while others would kick in after 30 days.
一些州，如阿拉巴马州，在1973年的历史性裁决之前制定的相关法律从未被取消。 ||| Some states, like Alabama, have laws enacted before the landmark 1973 decision that were never removed.
```
`zh2en_token/test-1.txt`:
```
一 位 医生 计划 在 墨西哥湾 开设 一 家 “ 漂浮 医疗 诊所 ” ， 为 有 需要 的 女性 进行 堕胎 手术 。 ||| A doctor plans to open a floating health clinic in the Gulf of Mexico where women can get surgical abortions .
保护 受 州 法律 威胁 的 女性 生殖 权利 （ PRROWESS ） ” 组织 将 提供 生殖 健康 和 保健 服务 ， 包括 避孕 和 怀孕 14 周 内 的 流产 手术 。 ||| PRROWESS , which stands for Protecting Reproductive Rights of Women Endangered by State Statutes , will offer reproductive health and wellness services , including contraception as well as surgical abortion up to 14 weeks .
据 PRROWESS 网站 介绍 ， 漂浮 诊所 主要 为 居住 在 德克萨斯州 、 路易斯安那州 和 墨西哥湾 沿岸 其他 州 的 患者 提供 服务 ， 目标 是 每 月 营业 三 周 左右 。 ||| The clinic will serve patients who live primarily in Texas , Louisiana and other states located on the Gulf Coast , with a goal of operating for approximately three weeks out of each month , according to the organization 's website .
该 组织 表示 ： “ 漂浮 诊所 将 接受 海岸 警卫队 的 检查 ， 并 设置 直升机 通道 ， 用于 运输 和 紧急 情况 。 ” ||| " The vessel will be Coast Guard inspected and will have helicopter access for transport and emergencies , " the organization says .
此 类 设施 已 被 军方 和 救援 组织 使用 多 年 ， 该 组织 表示 ， 调查 表明 ， 患者 愿意 在 漂浮 诊所 接受 治疗 。 ||| These types of facilities have been used by the military and relief organizations for years and the organization says research shows patients are willing to seek care in a floating clinic .
漂浮 诊所 将 在 联邦 水域 内 运营 ， 因此 其 活动 不 受 州 法律 限制 。 ||| The clinic will operate in federal waters so its activities will not be restricted by state laws .
上 个 月 ， 美国 联邦 最高 法院 推翻 了 罗伊 诉 韦德 案 ， 这 意味 着 许多 州 现在 可以 限制 或 禁止 堕胎 。 ||| The Supreme Court overturned Roe v. Wade last month , meaning many states can now restrict or ban access to abortions .
由于 在 墨西哥湾 沿岸 地区 人们 往往 很 难 获得 医疗 服务 ， 而且 并 非 所有 患者 都 可以 选择 前往 其他 州 ， PRROWESS 旨在 为 这些 人 提供 更 便捷 的 服务 。 ||| Because it is often difficult for people to access care in Gulf states and flying out of state might not be an option for all patients , PRROWESS aims to offer faster services for those people .
该 组织 表示 ， 对 患者 进行 术前 检查 后 ， 将 安排 将 其 送往 漂浮 诊所 。 ||| Once a patient is pre-screened , arrangements will be made to transport them to the floating clinic , the organization says .
加州 大学 旧金山 分校 的 梅格·奥特里 博士 告诉 哥伦比亚 广播 公司 旧金山 频道 ： “ 人们 对 自己 身体 有 自主权 和 选择权 ， 所以 有 权 怀孕 ， 也 有 权 不 怀孕 。 ” ||| " This is all about bodily autonomy and choice , and so people have a right to be pregnant and also not to have a pregnancy , " Dr. Meg Autry , of the University of California — San Francisco , told CBS San Francisco .
奥特里 是 加州 大学 旧金山 分校 妇产科 和 生殖 科学 系 研究生 医学 教育 和 继续 医学 教育 副主席 ， 她 希望 以 低 费用 或 免费 的 方式 提供 服务 。 ||| Autry , who is vice chair of graduate medical education and continuing medical education for the Department of Obstetrics , Gynecology and Reproductive Sciences at UCSF , wants to offer the services at low or no cost .
然而 ， 据 估计 漂浮 诊所 成本 至少 2000万 美元 ， PRROWESS 正在 寻求 捐款 ， 包括 捐赠 一 艘 船 。 ||| The vessel , however , is expected to cost at least $ 20 million , and the organization is looking for donations , including a donated boat .
奥特里 希望 在 一 年 内 开设 这 家 漂浮 诊所 ， 但 她 清楚 这么 做 的 挑战 。 ||| She hopes to open the floating clinic in about a year , but knows there will be challenges .
她 说 ： “ 这 涉及 到 运营 、 物流 、 海事法 ， 当然 还 有 安全 、 责任 ， 我 的 意思 是 面前 有 无数 挑战 。 ” ||| " There 's operational , logistics , there 's the whole idea of maritime law and then there 's obviously security , there 's liability , I mean the challenges are countless , " Autry said .
包括 得克萨斯州 和 路易斯安那州 在内 的 13 个 州 都 颁布 了 所谓 的 “ 触发法 ” ， 在 罗 诉 韦德 案 裁决 被 推翻 后 限制 堕胎 ， 而 其他 州 将 在 30 天 内 生效 。 ||| Thirteen states , including Texas and Louisiana have so - called " trigger " laws that would restrict abortion with Roe overturned , while others would kick in after 30 days .
一些 州 ， 如 阿拉巴马州 ， 在 1973年 的 历史性 裁决 之前 制定 的 相关 法律 从未 被 取消 。 ||| Some states , like Alabama , have laws enacted before the landmark 1973 decision that were never removed .
```
`res/test-1.txt`:
```
['漂浮/0/10', '漂浮/4/23', '漂浮/8/16', '漂浮/12/9', 'floating'] 
['诊所/0/12', '诊所/2/6', '诊所/4/24', '诊所/5/1', '诊所/8/17', '诊所/12/10', 'clinic'] 
['堕胎/0/21', '堕胎/6/25', 'abortions'] 
['州/1/2', '州/5/14', '州/7/23', 'state'] 
['生殖/1/7', '生殖/1/16', '生殖/10/8', 'reproductive'] 
['PRROWESS/1/10', 'PRROWESS/7/25', 'prrowess'] 
['服务/1/20', '服务/7/34', '服务/10/30', 'services'] 
['周/1/27', '周/2/30', 'weeks'] 
['路易斯安那州/2/13', '路易斯安那州/14/3', 'louisiana'] 
['州/2/18', '州/6/19', '州/14/8', '州/15/1', 'states'] 
['患者/2/20', '患者/4/20', '患者/7/17', 'patients'] 
['月/2/27', '月/6/2', 'month'] 
['组织/3/1', '组织/4/14', '组织/8/1', 'organization'] 
['法律/5/15', '法律/15/15', 'laws'] 
['人们/7/5', '人们/9/15', 'people'] 
['医学/10/12', '医学/10/16', 'medical'] 
['教育/10/13', '教育/10/17', 'education'] 
['挑战/12/18', '挑战/13/27', 'challenges'] 
```
