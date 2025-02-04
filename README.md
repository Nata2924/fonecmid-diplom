Функциональные требования
Выгрузка информационной базы (файл с расширением dt), включающей демоданные и конфигурацию с именем «УправлениеИТФирмой» из диплома блока Б, дополненную:

Подсистемой расчеты с сотрудниками, а в ней:
План видов расчета Основные начисления, Дополнительные начисления и Удержания. используется для учёта в регистре расчёта Зарплата, использует период действия и зависит по базе по периоду действия от самого себя, содержит предопределенные виды расчётов: Больничный, Отпуск, ФиксированнаяПремия; ОплатаПоОкладу, вытесняемый видами расчёта Больничный и Отпуск; ПремияПроцентом, зависящая по базе от вида расчёта ОплатаПоОкладу.

Регистры расчета Основные начисления, Дополнительные начисления и Удержания. Регистр сведений Условия оплаты сотрудников который:

содержит измерения Сотрудник и ресурс Оклад и Процент от Работ. Регистр накопления Выполненные сотрудником работы который:

содержит измерения Сотрудник и ресурс Часов к оплате и Сумма к оплате.

Планом видов расчёта Начисления, который:

Документом НачислениеЗарплаты, который:

содержит табличную часть НачислениеЗП с сотрудниками и суммами; при проведении формирует движения: по регистру расчёта ОсновныеНачисления, ДополнительныеНачисления, Удержания с указанием сотрудника, вида расчёта, периодов и суммы; по регистру накопления ВзаиморасчетыССотрудниками, УчетОтпусков.

Документом НачислениеФиксПремии, который:

содержит табличную часть НачисленияПремии с сотрудниками; при проведении формирует движения: по регистру расчёта ДополнительныеНачисления, Удержания; по регистру накопления ВзаиморасчетыССотрудником.

Документом ВыплатаЗарплаты, который:

содержит табличную часть Выплаты (Сотрудник, Сумма) при проведении формирует движения: по регистру накопления ВзаиморасчетыССотрудником.

Документом ГрафикОтпусков, который:

содержит табличную часть ОтпускаСотрудников (Сотрудник, ДатаНачала, ДатаОкончания) при проведении формирует движения: по регистру накопления УчетОтпусков.

Подсистемой обслуживание клиентов, а в ней:
Регистр накопления ВыполненныеКлиентуРаботы которые: содержат измерения Клиент, Договор. содержит Ресурсы Количество часов, Сумма к оплате.

документ ОбслуживаниеКлиента:

содержит реквизиты Клиент, Договор, Дата проведения работ, Время начала работ (план), Время окончания работ (план),Описание проблемы, Комментарий. содержит табличную часть ВыполненныеРаботы с колонками: Описание работ, Фактически потрачено часов, Часы к оплате клиенту. при проведении формирует движения: по регистру накопления ВыполненныеСотрудникомРаботы, ВыполненныеКлиентуРаботы.

документ ТГ бот:

содержит константы токен упарвления телеграм-ботом; идентификатор группы для оповещения.

документ Реализация товаров и услуг:

содержит константы НоменклатураАбонентскаяПлата и НоменклатураРаботыСпециалиста с типом ссылка на справочник Номенклатура.

