# กองทุนความมั่งคั่งอธิปไตยแบบกระจายอำนาจของ Acala — DAO รุ่นต่อไป & AUM ที่ไม่สามารถ fork ได้

โดย [Joe Petrowski](https://medium.com/u/9f4b86fbf09a?source=post_page-----80f8c23d8f27--------------------------------) & [Bette Chen](https://medium.com/u/8d475d21e811?source=post_page-----80f8c23d8f27--------------------------------)

**TLDR:** Acala เป็น DAO รุ่นต่อไป — DAO3.0 ได้รับอำนาจอธิปไตยทางเศรษฐกิจและการเมือง (การตัดสินใจ) ผ่านการกระจายอำนาจบนเครือข่าย Sovereign Wealth Fund (dSWF) และการกำกับดูแล สินทรัพย์ใน dSWF นั้นเป็นสินทรัพย์ภายใต้การจัดการ — ในขณะที่คุณสามารถ fork code, สภาพคล่อง และแม้แต่ชุมชน แต่คุณไม่สามารถ fork AUM ได้

![Image for post](https://miro.medium.com/max/1600/1*tG3vPiETDyoJgt1aC_5ygg.jpeg)

Polkadot และ Substrate เป็นพื้นฐานสำหรับรูปแบบใหม่ขององค์กรทางสังคมและการตัดสินใจ Acala ใช้ประโยชน์จากความสามารถในการกำกับดูแลและการบริหารเงินของ Substrate พร้อมกับการส่งข้อความ cross-chain ของ Polkadot เพื่อสร้างกองทุนความมั่งคั่งแบบกระจายอำนาจอธิปไตย กองทุนจะช่วยให้ Acala chain รักษาสล็อต parachain และพัฒนาต่อไปได้ดีหลังจากการระดมทุนครั้งแรกหมดลง

ก่อนที่จะเข้าสู่กลไกของกองทุนความมั่งคั่งแบบกระจายอำนาจ เรามาพูดถึงความหมายดั้งเดิมกันก่อน เช่นเดียวกับองค์ประกอบทางการเงินแบบเปิดอื่นๆ รูปแบบการกระจายอำนาจมีรากฐานมาจากการเงินแบบดั้งเดิม

ประเทศส่งออกสูงมักจะจัดตั้งกองทุนความมั่งคั่งแห่งชาติเพื่อจัดการส่วนเกินของทุนและความไม่สมดุลของสกุลเงิน เมื่อประเทศส่งออกสินค้า จะได้รับสกุลเงินต่างประเทศ เช่น สหรัฐฯ ดอลลาร์ เนื่องจากผู้บริโภคซื้อในสกุลเงินท้องถิ่นของตน (ของผู้บริโภค) แต่ประเทศผู้ส่งออกต้องจ่ายเงินให้กับคนงานของตนเองในสกุลเงินท้องถิ่นของตน โดยทั่วไปแล้วจะมีสองทางเลือก: ขาย USD และซื้อสกุลเงินของตนเองในตลาดเปิด หรือพิมพ์สกุลเงินของตนเองเพิ่ม สำหรับธนาคารกลางและเจ้าหน้าที่ของรัฐ นั้นไม่ชอบวิธีนี้ซักเท่าไหร่: มันเพิ่มมูลค่าของสกุลเงินของพวกเขาเองเมื่อเทียบกับสกุลเงินที่ได้รับ ดังนั้นจึงลดมูลค่าของรายได้ในอนาคต พวกเขาอาจใช้ทั้งสองตัวเลือกร่วมกัน แต่ต้องการลดการแปลงสกุลเงินต่างประเทศเป็นสกุลเงินท้องถิ่นของตนให้น้อยที่สุด แล้วพวกเขาจะทำอย่างไรกับส่วนเกิน? กองทุนความมั่งคั่งแห่งชาติเป็นกองทุนของรัฐที่มักมีการสะสมของเงินตราต่างประเทศตลอดจนสินทรัพย์อื่นๆ เช่น โลหะมีค่า ตราสารทุน พันธบัตร และอสังหาริมทรัพย์ พูดในสิ่งที่คุณต้องการเกี่ยวกับวอลล์สตรีทพันล้าน แม้แต่กองทุนความมั่งคั่งระดับอธิปไตยขนาดกลางก็ทำให้อุตสาหกรรมกองทุนเฮดจ์ฟันด์ทั้งหมดดูเหมือนร้านของแม่และร้านดังเล็กๆ

กองทุนเพื่อการลงทุนที่ดำเนินการโดยรัฐบาลดูเหมือนจะหมดเวลาสำหรับการทุจริตและผู้ร่างกฎหมายที่ผิดศีลธรรม ที่บอกว่ากองทุนความมั่งคั่งของรัฐบางแห่งให้มูลค่าที่แท้จริงแก่พลเมืองของตน ประเทศนอร์เวย์ ซึ่งมีมูลค่ากว่าล้านล้านเหรียญ ให้เงินบำนาญแก่พลเมืองทุกคน

กองทุนความมั่งคั่งอธิปไตยแบบกระจายอำนาจจะเป็นตัวกลางในการส่งมอบมูลค่าให้กับพลเมืองของตน แต่ด้วยความโปร่งใสและการยึดมั่นอย่างเคร่งครัดต่อตรรกะที่เป็นทางการจากการอนุญาติของบล็อกเชน มันสามารถไปได้ไกลกว่านั้น กองทุนความมั่งคั่งทั่วไปทำหน้าที่ในการเพิ่มมูลค่าเท่านั้น แต่ในเครือข่ายที่โทเค็นจำนวนมากมี _ยูทิลิตี้_ ก็สามารถเข้าถึงฟังก์ชันการทำงานในเครือข่ายบล็อคเชนอื่น ๆ ตามการถือครอง

# Blockchains เป็นหน่วยงานอธิปไตย

หัวข้อนี้ทั้งหมดหมุนรอบแนวคิดหลักที่ว่าบล็อคเชนสามารถเป็นหน่วยงานที่มีอำนาจอธิปไตยได้ อำนาจอธิปไตยหมายถึงรูปแบบของสิทธิ์เสรี ความสามารถในการตัดสินใจ และอำนาจในการใช้สิทธิ์นั้น ในขณะที่หน่วยงานย่อยใน blockchains เช่น smart contracts มีหน่วยงานที่จำกัด แต่ blockchain นั้นไม่มีหน่วยงานหรืออำนาจอธิปไตย ตัวอย่างเช่น ด้วย “Bitcoin บน Ethereum” สัญญาบน Ethereum สามารถเป็นเจ้าของ Bitcoin บางส่วนได้ แต่เครือข่าย Ethereum qua ไม่สามารถทำได้

หลักธรรมาภิบาลของ Substrate ช่วยให้ผู้สร้างเชนสร้างระบบการกำกับดูแลที่ซับซ้อนซึ่งเกี่ยวข้องกับการลงคะแนนเสียงของผู้ถือโทเค็นทั่วไป เช่นเดียวกับกลุ่มบนเครือข่ายที่มีสิทธิ์การจัดการพิเศษ นอกจากความสามารถในการตัดสินใจเชิงนามธรรมแล้ว Substrate ยังสามารถดำเนินการตามผลลัพธ์ของการตัดสินใจด้านการกำกับดูแลได้โดยอัตโนมัติ ซึ่งรวมถึงการตัดสินใจอัพเกรดเชนด้วย

ขั้นตอนการดำเนินการอัตโนมัติเป็นองค์ประกอบพื้นฐานที่ช่วยให้เชนแบบ Substrate มีอำนาจสูงสุด เชนบังคับใช้ความต้องการของ stakeholder และไม่พึ่งพา miner, validator, ฯลฯ ในการเข้าร่วมฮาร์ดฟอร์ค Polkadot อนุญาตให้ Parachains ใช้อำนาจอธิปไตยเต็มรูปแบบและจัดการการกำกับดูแลอย่างอิสระ ดังนั้น Parachain ทุกตัวใน Polkadot และ Relay Chain นั้นถือได้ว่าเป็นหน่วยงานที่มีอำนาจอธิปไตยกับ stake holder ของพวกเขาเอง

ที่จริงแล้ว Acala ใช้สภาออนไลน์หลายแห่ง เช่น สภาสามัญ สภาเทคนิค และสภาเพื่อควบคุมโปรโตคอลย่อย Homa และ Honzon สภาสามัญ — ถูกเลือกโดยผู้ถือโทเค็นอย่างสมบูรณ์ — เพื่อจัดการกองทุนความมั่งคั่งอธิปไตยแบบกระจายอำนาจ เนื่องจากการจัดการทั้งหมดเป็นระบบเดียวกัน ผู้ถือโทเค็นจะมีความเข้าใจอย่างถ่องแท้เกี่ยวกับการจัดการกองทุน และสามารถลงคะแนนเพื่อแทนที่สมาชิกสภาสามัญได้

# การดำเนินงานกองทุน

กองทุนนั้นแสดงโดยบัญชี on-chain บัญชีนี้ไม่มี private key ที่เชื่อมโยงอยู่ สภาสามัญและธรรมาภิบาลเครือข่ายมีความสามารถในการจัดการเงินในบัญชีแทน

เงินเข้าบัญชีได้สามวิธี สองรายการแรกมาจากโปรโตคอล Honzon ของ Acala ซึ่งทำงานคล้ายกับ Maker Honzon นำเสนอแพลตฟอร์มการให้กู้ยืมแบบหลายหลักประกันที่ยอมรับหลักประกันหลายรูปแบบเพื่อแลกกับการกู้ยืมเงิน aUSD ซึ่งเป็นเหรียญ Stablecoin ของ Acala ที่ตรึงกับดอลลาร์สหรัฐ เช่นเดียวกับใน Maker ผู้กู้จำเป็นต้องจ่ายค่าธรรมเนียมความมั่นคงสำหรับเงินกู้ของตน แต่ที่ไม่เหมือนกับ Maker, แทนที่จะเผาค่าธรรมเนียมทิ้ง Acala จะฝากค่าธรรมเนียมเข้ากองทุนความมั่งคั่งของอธิปไตย

ประการที่สอง เครือข่าย Acala จะปรับค่าธรรมเนียมในกรณีที่หลักประกันของเงินกู้ลดลงต่ำกว่าเกณฑ์บางอย่าง ค่าธรรมเนียมนี้ป้องกันเงินกู้ที่ไม่มีหลักประกันและใช้เฉพาะเมื่อเครือข่ายจำเป็นต้องชำระบัญชีหลักประกันบางส่วน เช่นเดียวกับค่าธรรมเนียมความมั่นคง มันเข้ากองทุนความมั่งคั่งแทนที่จะถูกเผา

ประการที่สาม Acala ยังดำเนินการโปรโตคอลการ stake สภาพคล่องที่เรียกว่า Homa Homa สมควรมีบทความทั้งหมดด้วยตัวมันเอง แต่เช่นเดียวกับแพลตฟอร์มการให้ยืม ควรสรุปย่อไว้ที่นี่ Polkadot เช่นเดียวกับเครือข่าย Proof of Stake อื่น ๆ ล็อคโทเค็นเพื่อหนุน validator และรักษาความปลอดภัยเครือข่าย หากทุกอย่างเป็นไปด้วยดี โทเค็นเหล่านั้นจะส่งกลับคืนมา แต่ถ้า validator ที่ถูกเลือกประพฤติผิด โทเค็นนั้นจะต้องถูกรับผิดชอบอย่างเจ็บปวด นิยามของข้อมูลนี้สอดคล้องกับความปลอดภัยของเครือข่ายเป็นอย่างมาก แต่ขัดแย้งกับวิทยานิพนธ์ของ Acala อย่างมากที่กองทุนควรจะสามารถให้บริการตามวัตถุประสงค์ในเวลาเดียวกัน Homa ประนีประนอมกับปัญหานี้โดยการสร้าง staking pool ที่ผู้ใช้สามารถฝาก DOT เพื่อแลกกับ L-DOT ที่โอนได้อย่างอิสระบางส่วน (แม้ว่าจะไม่จำเป็นต้องเป็นอัตราส่วนหนึ่งต่อหนึ่งก็ตาม) กลุ่มได้รับการจัดการโดย Homa Council สำหรับการตัดสินใจต่างๆ เช่น กลยุทธ์การเลือก validator (อีกครั้ง บทความอื่นทั้งหมด) และผู้ถือ L-DOT สามารถส่งคืน L-DOT ของตนไปยังเครือข่ายและเรียกคืน DOT พื้นฐานพร้อมส่วนแบ่งรายได้จากการ stake จากพูลและลบค่าธรรมเนียมบางอย่างที่คุณ--เดาได้ -- เข้ากองทุนความมั่งคั่งของอธิปไตย

รายได้ส่วนใหญ่มาจากแหล่งที่โปรโตคอลอื่นจะเผาโทเค็น โปรโตคอลจำนวนมากเบิร์นโทเค็นเป็นกลไกในการทำให้โทเค็นของทุกคนมีค่ามากขึ้นโดยการลดจำนวนโทเค็น การเบิร์นโทเค็น อย่างไรก็ตาม มันไม่ได้ _สร้าง_ มูลค่าแต่จะจัดสรรใหม่เฉพาะค่าที่มีอยู่ โดยการย้ายมูลค่าเข้ากองทุนรวม เครือข่ายจะใช้เงินทุนเพื่อขับเคลื่อนมูลค่าที่สร้างความสัมพันธ์

# การสร้างมูลค่า

Just creating this fund is amazing in its own right. This single account actually owns multiple currencies not just from within its own blockchain, but from other blockchains as well. And this account doesn’t represent a contract or any user or business or entity: it is actually owned by the chain itself. Pause and think about that for a moment. The chain didn’t assign a foreign chain asset to a user or contract; rather, one blockchain (Acala, in this case) has a stake in another blockchain.

Currencies and tokens can serve many purposes, so the Acala stakeholders will decide how to use their funds. Acala first plans to use these funds to secure a parachain slot. Polkadot has a limited number of parachain slots, and when a new one becomes available, an auction where teams bid to lock DOT determines who can use it. Most teams won’t have enough DOT on their own to secure a slot and will resort to crowdfunding by asking users to lock their DOT on behalf of the project. Acala will do the same for its first parachain auction.

But crowdfunding the same project over multiple auctions is not sustainable. If the sovereign wealth fund can raise enough funds, the blockchain itself could secure its own parachain slot and return all previous crowdfunded DOT to the contributors.

When tokens enter this fund, Acala plans to convert them all to DOT and stake it behind validators in order to grow the fund from its three revenue streams by adding staking return on DOT. When its first parachain slot is up for its renewal auction, it will unstake the DOT and use it in its own crowdfunding. Eventually, it will have enough DOT to cover the parachain bond without resorting to crowdfunding.

After Acala has its own parachain slot, it can continue the sovereign wealth fund in pursuit of other utility. Rather than accumulating DOT for the singular goal of obtaining a parachain slot, it can take positions in other parachains for access to their services or partnerships.

The effects of blockchain sovereignty extend well beyond a chain’s own governance. By combining new advances in blockchain governance, interoperability, and economics, Acala has created an innovative and sustainable funding model for their future that puts the stakeholders in control of the chain’s destiny.

# Looking Ahead

Through the dSWF and governance, Acala will become an economic and political (decision making and execution) sovereign entity. It will pioneer a new way of DAO — DAO 3.0. Just like Norway’s Sovereign Wealth Fund, Acala’s dSWF will reinvest its network surplus in foreign assets — starting with DOT and KSM and gradually diversify into other assets, for the purpose of gaining access to network security, long term wealth generation, and strategically holding stakes in valuable sovereign networks. ACA holders not only collectively own the dSWF, but also can collectively decide how to deploy the dSWF. The funds in the dSWF are essentially the Assets Under Management (AUM) of the Acala network. You can fork the code, the liquidity, and even the community, but you cannot fork AUM.

More details in the [dSWF Whitepaper](https://github.com/AcalaNetwork/Acala-white-paper/blob/master/Building_a_Decentralized_Sovereign_Wealth_Fund.pdf).

# Join Us

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

To keep up to date with progress on the Acala parachain launch, subscribe to the [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

# About Acala

[Acala](http://acala.network/) is the decentralized financial hub of Polkadot, making fast and easy to use financial applications available to everyone. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations. Acala is the de facto open platform for finance applications to use smart contracts or built-in protocols with out-of-the-box cross-chain capabilities, security and financial optimizations.
