# react-native-instagram-clone


## Developement of this project is divided into three main sections:
**[1. Creating layout ](#ui-section-1)**
    
  * [1.1. Mock Design](#11-mock-design) 
  * [1.2. Phone Mockups](#12-phone-mockups) 
  * [1.2. Break UI Into Components Hierarchy](#12-break-ui-into-components-hierarchy)
      * [1.3.1. Common Components](#131-common-components)
      * [1.3.2. Specific Components](#132-specific-components)
      * [1.3.3. Components Hierarchy](#133-components-hierarchy)
  * [1.4. Static App](#14-static-app)   
  
**[2. Navigation](#navigation)**

**[3. Business Logic Layer](#bll)**


# 1 Creating UI components 
## 1.1 Mock Design
For this project, design is done with help of online diagram software namely draw.io. 
Full design available through this [link](https://viewer.diagrams.net/?target=blank&highlight=0000ff&edit=_blank&layers=1&nav=1&title=wwdwd.drawio#R7T1te%2BI2tr8mz9N%2BwI8lWX75mGSG7exOe9ums729X%2FI44BDvAGZtk5n011%2FJYGNLx%2BAkkrCBzG5DZBD2eX%2FTOVfkdvH9H2m4evo5mUbzK2xPv1%2BRD1cYUxTY7BdfedmsEIq2K7M0nm7W0G7hLv472i6Wb1vH0yhrvDFPknker5qLk2S5jCZ5Yy1M0%2BRb822Pybz5ratwFkkLd5NwLq%2F%2BGU%2Fzp82qT%2B3d%2Bk9RPHsqvxnZ2yuLsHzzdiF7CqfJt9oS%2BXhFbtMkyTevFt9vozmHXgmXzefGLVerG0ujZd7lA2sS%2FfHfm7u%2FXtLb358X9i9%2F%2Fyv%2BOAroZpvncL7ePvH2bvOXEgRpsl5OI74LuiI3357iPLpbhRN%2B9RvDOlt7yhfz7WX5rrY3%2BhylefS9trS9y39EySLK0xf2lu1Vj5LNR7Y0gxzqbRa%2B7TCA0XbtqQZ9f%2FvBcIv0WbX3Di7sxRY0rwET6SOYfIs2AUUcWwYUQeXbGqCydYEK9RFUQRNQCAAUcpEMpuqN6uFk9w9ODvEt5AvMZwOg8iFQYV2g8oM%2BgkrgPbxjx4OQsrVByu8jpJAopxBFloMBUeVDosphn%2Fd1AcztH8BQaftULOgC%2Bg8D%2Bo8RoS44OX2EE7F8wVQgCNCA2LUIBqCFtLFhD80FDi1XkO2IySyAD5HbCjBLm4nl4%2F7BzCVYFF2uhy0HSSBziAeJLhxoI7EemlmS4PIx41BqVz8A3Dzbcl2A1BymClxdsOuh6SXBzqWyJGuFFt0RpXJoeT0UZr5LRcb0bHyA1pAbQDItUEJo%2F8z%2F%2Bft%2Fxr%2F9Mv9yM%2FqcfP32x8z2R7iPQo1J%2FQbkqE2YtA92P7ICLUmxYZWpEG2%2FzX92Pv%2Ff%2BN%2F%2F%2FM9v%2F6WLZPr13rsf9VCyOQJ3jhyHMdyO2Gzn2ECTmfRzMkskwLHnzZvQyfI0%2BRrdJvMkZSvLZMneefMYz%2BfCUjiPZ0v254RBMWLrNxx68SScX28vLOLplH8NiI4dwmw1GMEiFWNAXAIYUOGkgghQbSDXUXCFiTe27fFYkQQgtgA7IpOvSdipDkJqhB3BIuwAh8Mk7DwAdu6cM%2Fljwp6yDkT3v%2BukvDDKilD7NXsDsVffdxfZq9nm9025EbuvzV7lFQE37C7jVdbG%2BjW8NJE4m4dZtpUI2dconzxt%2FxDQNy5%2BNJG%2B201sqAgDguiDAjavQx8C0fczf%2Bi7POG32A2LJ6MaUBka2eLYtWUXF1LO2li0Q%2FhSMws9%2BpNoMpFQyq48%2BNShqgDv94y5EOTobbghW4XLt3PXOovSZbiIary12fDkecvrGW%2BhDt7CSTAX7pvmQpBve2Gu96C4b4oLdQj9nAZz9U5zQe7khbneg2JJc8koBpnL0YViyHN7j9fbylIS6%2Fj4gbiuzGwB%2FoA%2B%2BnrCjC52q%2BTRoTAZ8hzL1gV3DBmFZoWabfuhDWLGtqlXXOHMXBeDxY8eHxjKNBAAK0SXsMOQDfdKJ9jpKOwG4AK3UpEK3ItS0JFLC4yGTbHq2F8r9FZRGrN7jlL%2B2Xg54%2B932Hq8CGfRdbbaVI8WSC8rNQHWrWKJ2WaXmyTPkwX%2FIC0QmYd5nCwVIkwQowGhFukoRlVUzcBIU101A0T8bE3RoIA6h9JdRulftRUgqZrbW2Wg9FCvQam6%2BE0jKLGQRugbKFVXXLaBMkwn25p%2FZWZ%2BXwALVgT0MLeNiN9kawqEHfRls%2BHCCQlMO1OulzabCjw4%2FvFS2iAWVBf%2B6ExpV2XqR8hpg8AbUj0ADUTgmUtqg8Dr4BScRNyR8bwAeSqfIQBNe12Qhyz7jfP8ULrNnLNu3X%2FVnOqHnnvUSjCFm8XT1JW1pFHp3F74UaHD4Z7iWWGJOk6%2FsCT7JI%2FJfJ58i9LshNEgMYt%2FZDTI%2FswGDTwOdLpokLjh2GgAs%2FWV0ALCvJMNgHmIN509%2FMDui%2F2Pfbdde%2FUjf8kBZhdB4cdwEc9fNp9hG4WLVXGREB7se4rmzxFHiXSluUktsox5ZLlxbXOX%2FOIySRfhvLo8j3KG91FWBhiBt3DiGm3phF%2FekkrjcszIgCOdX7dr315czNNwmT2yTcvtGeWVb%2FiWpNPmt9c%2F%2FhBOvs4KIhsJYMWOX4GTeXW715QDV4yqM6KPeQbybhEzIirhuHzIVlswerfQqrD0IcriGX%2Fy7vrJgC%2FskCbHuMB5MgQZZCqSIzDLQF7YgUywSGTz6DFvo28fLv58XfoF3ORzkkYL%2FnirbM1%2FTwuiY7vFfE%2Fmy%2BcbKpskyyya5FG%2BTjd0spEHablPOI1XcRYXRI3taB5vP5cxWcl35YvxOlskU6s10fPWZHd3iZ4yev47fJiXsaxVEi%2FzghjozRX9wPda58kGZOrItYzEV0lWXyZXFyBXFYULMLnKfu%2FHaYHwX9OEqUw5gPNmL3irdJXAUTjf4foy2weQoqzOB6oHpOwD3zKSDie5OgiqTvnTHoKx3aE9lfp4U6EK1AwTe7hb6lifqOmQOjsR0Lt9A32HVNtpgJ72jurP5jQB7RvVd6kc640uFrN6HqCLC1%2FPHPg6JD%2Bzp3DFXxZFOU1giZZ3nqxqq5%2FDh2j%2BK7Ovt%2BU3D9u6nJs5v3BTub5QTV2zAqhIS5d%2FPMbfOTJvtvfz4SnPeeO5aw4JPJ5Ml7YVM%2F%2FlkbvsqTVh34jH0zAP2S%2B%2BnnGPg7nL0xFzmaNRlGUMo3E4H63jEb8%2ByrgTNKa8ln5cXb1nq%2Fe8Hd4IYd9acV9eK6kwp9ciArEQy917mJ5gC2hAs1tVTz34LKmHEUpBOiu21Xy0itJHtjXPzI55h5YxT4vfx9w3fWRC5v7Lp3v%2B7vuncB4uwuV9Fj5H94sw%2FcretXkdTePwnm1qhrLEACQkhMyKcM1pWd%2Fm%2F1SJ8AA3oOeXTXnq3j0CwOeRqkZQPQQ7VAUMjg%2Bdg3y4YOBjwpn%2FNXoIs3hScOD3ggnjxWw0D5fTbMIe24S8FmpCfeJbrrtPWkMhIFcbj2k%2Bzq%2BUx0T7vh881qG%2B9sJjejWXkAjoGY8RzRXYivUYZdZkA5wBAtjMZmYo0ERNJ6eRDjGkC6dp1ma%2BTB39YjbNheVaFRrMaYDfr5XNOgStLmxmVKH1jMccOba2TRjeTdIoWkrkMrxcrRDOdLyOyTFtIIciKq9LjQVQZuz2f7788sfvf10OXVaoLxtPlmnRjt0F9GH%2BFH14clgcx8td2HU0i5ZRGs5HyeNjzOgCj%2FnkgvE%2FNqv3o%2Fv%2FKdbvqdMeK1OquDGueruWPodNrTJCXw%2B9OpYLxV53y%2BoJpkPYbHAEgw4SDLLtjd4ePSbpiMdaR1WstYzAYjKaPIW5ISLxm4dZfYQtoKbT7EEXOdxTjYLonZhXoshFHCCosUVpS5vBgRwOOGkcYOG0lw84OWY16inGEU48O0WE4skWRi43btAR0kVHHUINg6MjfJCOVvGy8MEa6pXDYjxN8syMbiW22BoFGugDiXVtYRMHCpuo6AKW8cawZ9kGDDm0yfUe4IzparIHn3XV1aT0jJFMbb9nSG4%2F%2BHRB8luRLNYHHh3J7QG19yF5GX07P%2FQ6dt8EtRw1%2B4ltfSrxaaEHxNHD07SHo2mR7TahVAzP6diOTV%2B7HCq7%2F9eTPH6O85dToc5qEGtFnggCvFkKff%2FsDbhvpdTIocQmfFr2rXmWvqOcCryGQZR7RlF%2BcF7HpPJOd1gt3eja0ltNgeviHgF62Iv73lQn2J7QGIKC8hNKPWMF3SxhnLZ72e%2BbwfI5%2FhplJlCkdEIOEsavU95B78goctt95Peh6DZZ8BKN4WFJnBXQCyzJTu4v3HOxf3CdHzvoo6F6KrYncExwfEVV9j3S2aJXGTGLWsFFwaGmnWXCp9EUDesC5rnMwUC2L2AC%2BwcwQbCFTcbE3fbJGJJJ%2FD7dcLB7%2FFl1VkMEmOewlzKMJmBdKFqgggqyPGQwml7xxjlVxzD7JVkPq75NCQngZsDVJf4BEkCQmNZHAwr8cZAGxgXm2WWeIx2eqSjO%2B8CHtCsYVtVmNQ6obTuiTtPUaxvHYFT0dSiu7w8Ag%2F4B0IO8y74C0OkjADt0djjrIS5EaPPcOsXFkbGmYooLjDXNLqJashc6CQRwvMMs2WtukK8WgELJZC8AaGwE3kDlhphuND39CW5pjSQkRdNZdLf9M0nzp2SWLMP5x92q4I3s3vM54SWKBeT%2FE%2BX5y3YaDE8nNVEbfY%2Fz%2F91%2BnL%2F%2Bi7%2B2PLr988P32rUPL%2BUfS%2FbAxacsTMu%2F%2Fyp35H%2FsPlf89XIIeVmyTifbpwZH55TGNgfJXhyn0ZyRy3PU2B5C1vajv%2FKcW92SEkI1AbWlA5ybu91%2Bcod2YDPRqqBU2ow5wrMolzYraKh6rneQ1ZDUESUi8I8vTf1BqSOJeo0CcC%2FrDmKsHfXdYwIQpkBTnqjysWEEEYvK8OzP4DBPc%2BMqtSMXMZKg6R44bW4WmppbFCkVldjrOzQ1N6NRCk3Ue2gOKR6Kdq27ewrNIQVHbc%2FvNzQDzXJTb1WBj3pVVRB0EJsnWlUQ2D2rKgg6TFO7VBUYqCrwD6WUzY4NO1jue6kqUF1V4Nl2r6oKAsiCuFQVSFUFwSHtarSqANkGgjkKTZVmhyivzHYdzThBpal5DtaJAHwqh9FM2yOonMF%2BMUhMGyTCqVOKgC4QZodm2u0jAC9WiLpARhPvLgHwbtbyQHZ7rfN5mx6CxUhlbWnY2BhWXCQQoky%2BDR5YAS2OyrDSAMUzCohIKEA2hALzdsclEHIsu0OiCLAdmWHT4%2F0BELBH8GRz7pKDkL1HHBb9pvHGbeOHK%2FJNa6R1aDo1OLNY%2BtRuhvGbvuRKnH3cnHQs77lv9nHbTcBdYw7f7bkZgHYg5l5851CHdOR4FjCwonTe1bMj6hDUkPry1ZAD9G0Q0VB2FeRo39ZYMDNg190vXjDaHM9jJpTH4d%2FrNOLPtO2lzF594m%2BzsmegWZ%2FaEgPSLFjzkVsND6lLS3hIXWlAasAQ5KsRck0%2Blj1aB9ySY4S8ZtAP6BEEnjjXpp%2BAcePvN1fAniwfwpR5SvbPyVSxxdJ3lAtHFxxStRk%2FVt8dBMxG14T1z8XjyHr77MhAbL%2BEj00CkK%2FIhOxH%2F%2BPH4UObHBSzRptJVL3Ea9B%2BqNoFy%2BwxdPBjSc1BMs83iwI5H1PAdfjAdoSSJ1DBELPAxpB0scvQ15DBjaQjRRC4zUYZgJmyvDP4VdlNbfBAx8KAu8puPZ5EhwxnUjSpGzqwkUDgsqliWJhA1ioJH8MojE4A2oKuZMY5kDgz6xWC83NJhPm%2F4UMci7LEhSS4YYjLaYPVZnwfW3xY53kx56EMoQ0a%2BkKf5KoxbWO%2BplngQ0F6wjyh24%2Btxrj%2BXskjfBhQEJESfXCCKvmI4wQ2j6b3Bk5lP5cDtoE%2BOAHnICFmPgVRKjJzOYHveMxMZD%2FvhAPIyIHKbMzqLgKG7I8uFiRQudhCsp43LBpktyHLw3ydPYTpCblrvmBiBSDozUY8wVH1pxrxRIEHyAWzLjI49v10JTEIcbOSuMuYWdMjPxzkWV5THFBblgXwxA9fH6gurZNei7aAyMad2c5JqMt4x76cRqakeSwioLJ4MHr4GIHjEHsKPUcYXnJ86IFzBhVCryrv2TVnoYpgGaC%2BwVJ1w0tjjW6o3zeuBqfmDQKWLgGaXxwbmpo1jMoiPkcw%2BimxLV9OjCHQz3Kl%2FnTqgAiOmxGAOLgpzM7had7fi2ne7BXPDo6zSbhcMlOtffyySmJwMbEoEugBWWV38IbNZpWWQIMidssaKKKDwD9BisjycDkN0%2BnoMY2iUbmKuGU4HrPP2cgMcYhaiwKlvsiXaQJps%2BRNzNdRJ2fFllfUdS2ghG838bzBWI5Vphw1wLFD08rBMZZ9kLG%2BMfgtR9lTEmWFzB0VkdPRKl5%2BfRk9htkTv2E8pvwE3vhP3kv2PltG4dcoNcNwjiOIYhdDBAMVUugLPrua%2B8wpBaDQnpNzXDlosM5xkCJzLH3sNiDzkAo1x21CyzAIdU%2BLUGpU2SIIPasc1nDosLROEHZQnico9B%2FWGRP1WcaF%2FZztyu5vhG1eOjPmHsd4Eqb5iBoS8IEwP5IxF9RdkFo2YFfVljVQxymaBPggdUzWeTTKo8lTYWePsigfocoE%2BCkKp6unhFGPIYObEisQbUbfKhsCNMIbFoEoZLesgUI65IkGRyHkIIU8MfAyAzCaridFtqQiFO6T8SKw8UOSfM0M%2BOolHdTVCtBO02lxJ7QpFt0zBLRGv8BOd4BmLhW4BvCdZ5RjwZ2xvPhr9BBm8YStEfydcHDGi9loHi6n2YQ9tgG1XIq2ahIuVB9FsEwV5ZoGqhhQ63lKRabyoOJosKYPUawxptxlOseFt%2FQGEQXeoi7UYMUwcxnoHKUvjuiWBS4N3gKjiK6vUe13CAxdeEuv3qICaXhlffjxWEt1iZRR1vKozzTX3u4zNnPZAU5D%2BlzzYECxL%2BqIPdYOgzQAYonI9io1oQGiF5P76KJLOOy%2FawR1NNEVXIzFoxuLRKAK54DsMEwhst14F4Xp5OlukkbRUqKWodWni%2FFpB%2BiBYvb8BTgi5D26TwGUPDFFZpPO82GdQB%2Bo5Czj9XTKRE5%2BItTpo6Zl4XhgA13DRwdVTKoAu2BJzbVu0yjM%2BWlQjlO44dVb%2B0f2HPHCYV2KQcQblUzYVl0Xf2JnQUQp2Ysp2rhLL8%2B%2B%2BFI%2BbVpDAT3UGtVo1TNGpurxFcAyoD0fQFm1fR9eRX4g1Lv0jk4HNKLbt3s%2B2hODzV97Ck0ee%2Bo3NLtMPx9czOFw2c1znK3D%2BShM0%2BTbyC5Kbop4Q7Fwz1vL30%2FjdFOtdc%2BbXpopwPHKYtHK0AQMFiDiUK5poI9TjFQOlj6k6bYUBVWZfmOGC1iDg7Ql46qYV41Obp%2BSJOPu4iycz6Ptl6iS0i77UTUbx0dNrvMptQL5SF8ZtG%2BANLDKmnkNMJXthuvptPK%2FhwLNAFtAgyXz0DzF8kF0UJLlafgczTfHTWZJMmWvHqOqwnQSLqI0bBdeSgmjNHaqSgxw2BqGTnRpG%2BKFwQY7QyeLwSo4sTxyhHzLc3bmsg0cDDVrD71%2FNBL2O0VbPyezRG2QdaBDehwh%2BuoG0IEgs%2B19q1bZurzQj8W%2FNqRp4DTk8gOf%2ByY5Y6gsmegr8KrGTewb%2BPGlmidnFyO7Pi7CeH5eU%2BRE%2FkAksKhfwySgZA0zS%2Fso2wo%2Fv4ZZ9i1Jp2eGO4ELeYeL%2FVxotDcb7tKbDbCGWu0eCfwdDCHYxNog%2FM8tYLBEAkUkz7fHtpiWmobZU4XC0rJbfJ8xDD9ZcZJ5he2UWdGS2c3JKrr%2FIVqs8pcf98hoFYQgZKuQx4xje684NksIULHtK7PMtGn3bPuG1j%2BxQ7tkH91x5GP709LE4GJ0zf%2BpYnEx80OwB3W8AfUrM7r1ucRgO8EuAywVLpETHCRELaFbP2PnY7fZxGAXQrL5GT7MkWf3EuhykUa8XK25vKyP0jqVFspEmMICowAZnTOEgRaIvyQcAyH7%2FyJaPETccbgiY%2FZfrmXWK%2FZiyeyFflqdXOkJ6crbW0WqSpgSRXj6EjifapaHqOr0uQJIeUIp4MhhMv9AnMpsOSampxjvHmxg0yMCwSDmpNcry4GIltHAJoWOJF4Cmzqdfw%2BL5yqbcRugq6jZuA3V3HpLe5BT5DrkEsvBOwj7AIhNRzmp5gOLxoHMzAjLJzUgAzUsxoHcnra5hJLbJRJiOPH2hiMNR5Kp7E9dIskwF2J0SNSZNeO7tFe%2BhJJVUIIwWhl52HK9%2FUrPLCWcYk3h%2B9oq34WPUf6yr7GyWgppVuJgii17f8YQqsrRV5QD9Ae%2BnqdROOUP8RQ%2BR9voTTiZMFzmUKC5CufEy3MN53jEEzMP1LWwU0M0lIXwwNpRfdJAtZOhAHJIiGOOytjN4XhOUEXM1IPKO%2BijvyqlVn42W4XLLv69mMDbJea%2BrGrG1ma71%2Fn0fUnWIcmK8g7VUrSl7coGZBrIQEEuFjzxy1HZPcF68vITUYEYXAzVhRsOh%2Fsd7OhexwukmheKDlofxkvPOjRou5ioButhMHWsAB%2FZLO0yAGxwVHG4A%2FE6i9JRzEX1I5Mho2SdF6cJOAbHLp8Z9O84%2Bna%2FhzC2RQZahbUrpp5d1NTcMu2YFduyS%2FNnNGfwjk6kOwryBZsZ7BJpFuZyCnRj4pwIyB3fPwhys01JgMamG%2F%2FgRCAunmE6PsTVN2cUZTT%2FkWX6uPhR5XU1RYfvdBQd%2BqonunRo7DtYMZXAaiHAfzEM2Q51KWyfeJW1OYA1qDZR0NrBSADyoz%2BJJhMozv%2FgUz7DVw1VC9VUPrUPtH6A6uIcfYhojybtWn4l8yJ%2BepM8DCid1sZrKpCKxZiq7%2FsWgZrNG42iBgpiQjYUExon8zkPnuuP403DyH%2BUuVJd4AFRX6wRDpCsaRwKBcAR1TcmgNgdtM1JyETsiyrpUKsmozKRlO3LLzLxNUh1ZJnoHl8mErv92OFFJpa482SZCBQvH0MmQnaiwIqvrlAF0XmbLBZ88KrNXqwYZLkXWX5TKpWxSisS%2Fi8ygXeyash1u9lJEtmBrHeZ8K2SZoYExPtrnpUcamykTweRJxWrzQiW8Wn8PCPp0hL3Ep%2BXKcNEfD4QTsxgZowHqDfxeQI25r0ccO4iC1zXcpuBaESgghnj8gBsEHwplFDO256PZAoANLzZSgkCdjR%2BpwWJwDNON2umC5YbsS2WIqo0EjUmR3Tagq5MHhggD6OJE4KgIyEKRaz2OhqEsYVozcbGAgcCw1NMF9IQdIom2ZAKaRARqISIVEKgeZhGC2sq7%2BGkqOREDHfultcJCAn049tAiweztjtut%2FMUK%2FpPm%2BYdF52OsG2h%2BkmCZtNfhIHCCLPWH%2B6Q3lRDFD9FIWNxLkh%2B%2BDPOn5JNe5ckZYs%2FXmilOE3ROIAm0ooDlHuYJpYOh1BeP4inKOTQCljXooLV53jQIEtm91kOoNL1ZdJwB%2FN6cCp9sO1HmL%2FFKKVmBToC1fhQo6YSZUY6kJAuo0j6yIOehQTnljoItIkCywcgqo8HL8M7%2BsaDyG%2FnQUpBS9osD6rutXUw0qna3cXI8kUXt2tySmcgpMv4iUv7AxUUQCAKgMfkGLUxiYJs82VQ637cM%2BO3bG%2BxE6uQMjYbayaye%2FFpmeUhY5VFB6APtCUNxa7lOK1uH6KBJdeIGe0NSrpMf3lPEqAaeqsAnA6zKsXWLsjFAAwNyzXNiRSVMHSZcng1SZoFp2MsmLmJW%2F0cxssfPrwsw0U8YW%2F9xFX2j5c0JjRnQ2Q%2ByK40G7cCJ2sI8D%2BJwnHHseUcsutZnqzaIR%2Fbt6t3akDCuZxooo5ruYJpjX1oihvcG8fCjjYcGIv2Xz%2BHeZheBCIwQopJPyiX7JkVie8%2FCUXAMvEr3Nlv0sztKg%2BJOlQuznGAU1E%2BgERfHxI79GtVxM7FRNW7POG3feFphzh7EwVQUZHZrg4EmKlxYfA9StslMoM73RxvfakJYCiHmrNZXfj5ZAMuQKGlA1TWQ9aZPn4FuyZdUP3eUS2%2B5bm9QzUGUK0wFKR0IofvNNJxQl0bolCnDNeCjrAiW1tlJDjFRYshdBum04sFBB9nQYBBbDbQA47iUCFEP8dfo6yr%2BHwv7yobJe%2FJOHJ8WfqBONLHq%2B%2BfDQ4n%2BDbHS9jl6zV7sq6h2RPlTx%2FRSgjvy%2FCbzfDtGUyhBvdnjnTsCi0mkINlH8asTAYnWrylHfebDeDiJq8nefwc551t4PcIcd%2Fm%2FxQpWs%2BRKueOL8TB4RSvZGQMIoujKTo3xvW8QEay2y1hoJFzIT9FBZI%2FLc8TzaBBBqDZrID22tGs2Hn6g%2BPx4jwxT0lID%2FLKWgcfmd09BY2gQHbfoN1%2BQvjcGJ4h2iJCboDP4HZqLT3kNlKG2b89dqII7c75oR3LwZHAbgwVOjraFdTZ7ke7e35oF6s%2BbL9frK4gPLYf5%2F4Z4lyuuMI9QztUvqsS7fzWzw%2FtomLHTs%2FQriDQuh%2Ft56fYPZnbe2fPKYix7kU7OT9u9wAz3u8Xt%2FuvLoh%2FY3NYkDbu8mjFL1rsPwx14Vf2%2B8unK96oL0%2Bumj1j7Z%2FiKA3TydOhUrJLE9lu9Sy%2BdJLPBnpFUM8z3Di2LDE%2FKkkiTpIfmDAp%2BkZer1ZbynzVyY0LJXaixBEf%2FWjXf5q1NyPoLMgR6PJQoOttg1%2FhttkSxd%2Btokn8yE8RNUlQbqvdchYVmhzbgUDPjRjdwEJ1YhREpAsUq5jvre23e%2BTT%2BBmkOo640RYHnOx4p4Z2sussQ7udmRaG8b3izHS1XDxXc9Xwo7bxqTQdXVgasbXPySx50zO%2B%2B%2B4UQqrzKGtQsRqF96awY1PRYx%2FIGu6VkDBWWvYYEEE2AHQwsQrD4txUQ1n0VDZZh8xl8DxzVeGoQRO0B%2BneI026ifXmvE%2BVUv0IHLFrNHhEQT0gEbvt1mn%2FEC3CeF71YmyYlB32eaVQbny8uoVVmGXfknT65rvYpzBkI3kgWHodcA9qhZ489as96xa1rtnNKXR8XzUZcYiFPEGbYflMBkEU9GyQtgmmxG9PP5hRaLtxyheFdlFoF4XWIyxdFNpFobUlMxxBmxHAN0OBhQ1rs%2Fasqn5t9pOmkNvRdBnvpnVEXQZs3BMR0gWE%2FCh3vOc04hvCYMMFCLzEwfSqliXnDSrlQNoXVj0CxwgNXvstJdvRxB9jIz9BY%2BN9G98k0xcN246TJH%2F7%2FfJdNmOko7TbyXu9ce1em07IpmIhyC6K3bCeXItgIMtJtVlPpV12nFhAxIuNTsR%2B2jxMxwFLfbrvSbisDmkP57ZvwzyaNcwtRbJxt%2FGnPFoMCiZcrHewPntyx1t4%2Fx4up8niLbd%2BXkqEUCy0ENgNgeigQ1CgbUxx0F7gql%2BHMGeC086JKJF3BpSPJ4wXURoO65bZXmkyLycfD%2BXWuy3t4rJXeyPT2r%2FtIsmhSGogtaHmYru7KPf0uQPtheEGRPm2EcxFlh%2FztkssjON5LT7Q%2B1t%2Frai6ns%2FFxkNaReP%2BPnVDh%2BZtslgIBfL9fkB%2B692anvTohivWLAJv8XL2hshbP55gSy%2F1%2B38%2F911Mjvb%2BRg4%2FCiuYHBTwHqlv2YHR%2FG3QfuZHv8nxa5owlJo6NSHeo%2FGs075H6fx9bXetOqNsFop6d%2BkkGx%2BSfaFjUdi9R%2FipeKpRqfmXOcPw%2BzJJH6dxXnmQP5RFRG%2BrzNpuWdzXpLZr655A5v4tX3g9nTaytW%2FZo2WD8nmY%2FG%2FLMtbe8uZ8YW2PvaHv81KdCGFiYdFdB86lEDewPOiMogp3fU2iP%2F57c%2FfXS3r7%2B%2FPC%2FuXvf8UfRx3GY%2Fel4zWPXiOvNrhQ6Ibr2cTyEBACqYafNuZ6%2BOWYQ%2BUwbQ%2BAdBWXcK%2FbLA8ZrHjhy2NpvfPHT9bm2Kwnox9I4FjuPlJAgRXIpIAQlBnXxVrnMpeQ8JEre%2FkyqByHuqzDlUhsDCAnmtDhtHKlZKm%2Fj03XWZQuw0WHAPbD6XOqY%2FsHiMODOFXXCGSQMhQ0SwQJYRNj4QGufQHcnmpbyrTpfhFrQ1wNdrVV0KkcNl6MzQl%2BY9jsNQw%2B0O5ZzLry6Y5KygZlVScOF0NkUpUdGGHwUvMOw8rdr0192gJQKMtna4PoxbjZooNd74Fxgy%2FWTR%2BtG5%2F3zDqydYPfb94EECFMNvkXDs7rtlhi6%2BGJbr1WPicpjyFVYedXhaKY7FnzD08LCmI3EefApxgls%2BXbt37JFR9ws8yiSR7la%2F4t4TRexVk82fjm8p7RPN5%2BX1Z48lPeQDGK19kimbbdRMlQB3uDKZqPNFBmJJ69nxmDwPKcXc8wLPElcjwwVOToYk2oQZiAnjBbMepirx%2Fj7xxadUQBhp%2BIkngRzqItR99tLUK8W%2F8QLxidjucxE9bj8O91GvFHmkXLKA3Z7Y8%2F8bdZ2fMMNnqUlTPZdG9oz3c9y5GnqjtAqJRpXqKgTBXGV3sbH03%2BBpDkPm9vI7AIafc2fAIbx7qmc8NUoqBHM0gUo%2BvnMA9TIHPzZWuUfVo%2BJm%2FVYyPRsnv1Blke5msgAbZN8x1IyrXrvVeqr64poV4RNi%2BusGuE3Twoj9wADJMhKNyiz%2BsrT%2BufHWVvbV3g%2FgoFefbUS5rquxw6tlPf1PLxXsuLAISsomAIpOM9s%2B8qHcrd91v3X%2Bflz%2FKJosIJIerK2DLqv7rnEmpi3kcgAp92GxOp4nAvDPwOcSWHR7XOikuoQ3rHJXKUp1YkcE6Y8I%2BNCdmpf9x2OchOFxO%2BJx4tRR7xLJ%2FutP6R46DuXucdsFy3k6u51ZrOHn6wC9uQR%2B5qr37kLwsbsbBzH8NFPH%2FZfKayI5maIA5HcjR%2FjjiKpCvNTcSeMo1rm7vkF5dJuuAxmu3leZQzOhhlDM%2Bc5aG3iEHXLek0LseMLDgR8Ot27duLi3kaLrNHtmm5PaPE8g28D17z2%2BsffwgnX2cF0Y0EsGLHr8CJnWD3mnLgio4CYwJeCmzfLWLeLE423r3bDiZ9MTGkcTDpoNY6YFco4SBf4iBuN%2B%2FlINABJNpYqL3r5ysj%2FTC9g77haz1McJMykwAmBWpJgGYwX%2FbrmuH9fcF863C8rhnPP2bITgn52hL5%2BuQQ%2BUJjtBxt5NsemDtvt88XHXYP9Up1e1Dc6RRdwAA7IiLsA4gw6g6W5dUXd7COtLIZdl%2B5R452nYFrKGOlX%2B7InsnsqnOJ%2Bw%2BFnU%2F20HWoaKK4AbZcex9ReEaJQkEpMpxgKRstZgy268VStmw7uE38cNdyvXgoAhlv%2FHxeOzD%2FyjTMJWcokrNrObWaCUHe%2BT62SjvpkMmtLdOiYig9TNBX5eHgN5OiKpZoy12qug3%2Bpi%2BtGUx%2B9UOUTdJ4lccJ%2FBQXNmlnE48QC%2B3VAMiHkuz6dEB7kOXNhgF8wH%2F%2F3OY3UdBg7H6NBBfYFqnZmWW2u5p5AHRc1DmbFCQysEmXgKjsKVzxl2UJYQ1jIuDzZFVb%2FRw%2BRPNfGXsXAol8eEjyPFmwN8z5hZsqFFx3r4ufq21d4nVZ88gxIhVAlqWLT3m%2Bygr6HrP%2FTaZLx4onyfKRh7BTa8K%2BEY%2BnTDSzX3w944BKeBlH8dfoIcz4nN4xwd95h7RxvJiN5uFymk3YY1urpeaSRx8jS4i6oEAucYSat5Vr76GK6%2B%2B%2F3Xz85%2FPX7Po%2FTu5%2F%2BXsxcyLw4PKFKJpEAaMZIIZWzGO7OdMLlQWD9agOgHb6erSzP9OEy%2Fzq2j%2BYMHz6OZlG%2FB3%2FDw%3D%3D)
## 1.2 Phone Mockups 
![authdesign](https://user-images.githubusercontent.com/41279178/101013190-bb0c4c80-3585-11eb-8b35-272762297ab3.png)
![main](https://user-images.githubusercontent.com/41279178/101013427-150d1200-3586-11eb-86dd-6b669f342d3e.png)
![profile](https://user-images.githubusercontent.com/41279178/101013607-5ef5f800-3586-11eb-9ea6-aa689a60979d.png)

### 1.3 Break UI Into Components Hierarchy
#### 1.3.1 Common Components
![2ed](https://user-images.githubusercontent.com/41279178/101022229-e47fa500-3592-11eb-8e1f-cff9c9d97cc8.png)

#### 1.3.2 Specific Components
![ss (2)](https://user-images.githubusercontent.com/41279178/101045470-1fd5a000-35a2-11eb-8832-0f6024686bb3.png)

#### 1.3.3 Components Hierarchy
![hierarchy](https://user-images.githubusercontent.com/41279178/101021407-b51c6880-3591-11eb-96c3-c18ca2d60abe.png)
## 1.4 Static App
![Untitled (9)](https://user-images.githubusercontent.com/41279178/101048436-6fb56680-35a4-11eb-85c1-267c72730806.png)
![Untitled (10)](https://user-images.githubusercontent.com/41279178/101048826-c6bb3b80-35a4-11eb-804c-6c2d2941692f.png)
![Untitled (8)](https://user-images.githubusercontent.com/41279178/101047791-f0279780-35a3-11eb-8fcd-1745bd29fd35.png)

