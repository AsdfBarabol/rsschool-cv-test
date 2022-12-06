# Andrey Barabolya #
* ##### Contacts #####
    + [Email](andreybaraboi@gmail.com)
    + [Telegram](https://t.me/region_6)
    + [GitHub](https://github.com/AsdfBarabol/rsschool-cv.git)

### _About me_ ###
I am 38 years old. I live in the Republic of Belarus, Mogilev city. Higher technical education. Responsible, goal-oriented, easily trained. There is experience in developing applications in C #, for personal use, to facilitate repetitive actions. I learned about this platform from a friend, read reviews, decided to try my skills in Javascript.

## Education ##
**University:** BELARUSIAN-RUSSIAN UNIVERSITY
**Speciality:** automated information processing systems
[visit the university website](http://bru.by/)

## Work experience ##

>[![Могилевгражданароект](http://imgp.by/images/logo2.png)](https://www.sipm.ru/ru/)
>**2009 - 2012**
 + electrical systems engineer
    * development of project documentation

>[![Стройинвестпроект](https://www.sipm.ru/images/logo_transparent.png)](https://www.sipm.ru/ru/)
>**2012 - 2018**
+ engineer of the group of fixing violations of traffic rules
    + setting up complexes of traffic violations

[![Альпиндустрия](https://alpbel.by/wp-content/uploads/2019/01/alpbel_logo-%D1%81%D0%B4%D0%B2%D0%B8%D0%BD%D1%83%D1%82%D1%8B%D0%B93-1.png)](https://alpbel.by/)
>**2018 - present time**
+ cellular engineer
    + cell tower maintenance
    + industrial alpinism

## Languages ##
English - A2

## _[C# Certificate ](https://www.sololearn.com/certificates/CT-TLIAAJXS)_ ##

## Code Example ##
```sh
private void companyIdValue_SelectedIndexChanged(object sender, EventArgs e)
        {

            var people = from p in db.People
                         join c in db.Companies on p.CompanyId equals c.CompanyId
                         join pos in db.Positions on p.PositionId equals pos.PositionId
                         join g in db.Groups on p.GroupId equals g.GroupId
                         where p.CompanyId == companyIdValue.SelectedIndex+1
                         select new { Фамилия = p.Secondname, Имя = p.Firstname,
                                       Отчество = p.Surname, Компания = c.Name,
                                       Должность = pos.Name, Группа = g.Name };

            employyesDataGridView.DataSource = people.ToList();
        }
```