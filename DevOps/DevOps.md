#вопросы_с_собесов #devops #cicd

#### Что такое DevOps?  
это инженерная культура, практики и инструменты, направленные на сокращение релизного цикла, повышение эффективности и обеспечение возможности выпуска релиза в любой момент.    
#### Что делает DevOps-инженер?
DevOps инженер отвечает за автоматизацию процессов разработки, тестирования, развертывания и управления программным обеспечением. Он использует инструменты и методологии для ускорения поставки программного обеспечения, повышения его надежности и безопасности.DevOps инженер работает над созданием и поддержанием инфраструктуры, настройкой систем мониторинга и логирования, автоматизацией процессов сборки и развертывания кода. Он также помогает командам разработки и операций сотрудничать более эффективно и интегрировать DevOps практики в их рабочие процессы. **DevOps-инженер** — это специалист, который помогает ускорить разработку программных продуктов. Он является важным звеном между командой разработчиков и группой IT-инфраструктуры.  
#### CI/CD 
или «непрерывная интеграция/непрерывная доставка» либо «непрерывное развертывание», — это методика разработки программного обеспечения, реализуемая благодаря инструментам автоматизации  

**CI**/**CD** объединяет разработку, тестирование и развёртывание приложений.  
#### Agile?  
Agile - Культура поведения внутри команды
#### Варианты CI/CD пайплайнов:
_1-ый вариант:_

1. Интеграция и тестирование кода (Code Integration and Testing):
   - Интеграция исходного кода из репозитория
   - Запуск автоматических тестов: unit-тесты, интеграционные тесты
   - Анализ качества кода
2. Создание артефактов (Artifact Creation):
   - Сборка приложения или компонентов
   - Создание исполняемых файлов или артефактов
3. Развертывание на тестовое окружение (Deployment to Test Environment):
   - Автоматическое развертывание приложения на тестовом окружении
   - Запуск дополнительных тестов: функциональные, нагрузочные тесты
4. Автоматическое тестирование на реальных данных (Testing with Real Data):
   - Тестирование приложения на реальных данных или симуляциях
   - Проверка производительности и масштабируемости
5. Ручное тестирование (Manual Testing):
   - Возможность проведения ручного тестирования на тестовом окружении
6. Развертывание на продакшен (Deployment to Production):
   - Автоматическое развертывание на продакшене после успешного прохождения всех этапов
   - Мониторинг процесса развертывания и откат изменений при необходимости
7. Мониторинг и обратная связь (Monitoring and Feedback):
   - Мониторинг производительности и доступности приложения в продакшене
   - Сбор и анализ метрик и логов для обратной связи и улучшения процесса
8. Управление версиями и обновлениями (Versioning and Updates):
   - Управление версиями приложения и его компонентов
   - Автоматическое обновление приложения при появлении новой версии

Этот вариант пайплайна также охватывает все ключевые этапы от интеграции кода до развертывания на продакшене с акцентом на тестировании, мониторинге и управлении версиями.
_2-ый вариант:_

1. Сборка (Build):
   - Интеграция исходного кода из репозитория
   - Сборка приложения или компонентов
   - Создание исполняемых файлов или артефактов
2. Тестирование (Testing):
   - Запуск автоматических тестов: unit-тесты, интеграционные тесты, функциональные тесты и т.д.
   - Анализ покрытия кода тестами
   - Проверка качества кода (статический анализ, линтеры и т.д.)
3. Автоматический деплой на тестовое окружение (Deployment to Test Environment):
   - Автоматическое развертывание приложения на тестовом окружении
   - Запуск дополнительных тестов (нагрузочное тестирование, совместимость и т.д.)
   - Подготовка отчетов о результатах тестирования
4. Ручное тестирование (Manual Testing):
   - Возможность ручного тестирования приложения на тестовом окружении
5. Автоматический деплой на продакшен (Deployment to Production):
   - Автоматическое развертывание приложения на продакшене после успешного прохождения всех этапов
   - Мониторинг процесса развертывания и откат изменений в случае проблем
6. Мониторинг и обратная связь (Monitoring and Feedback):
   - Мониторинг производительности и стабильности приложения после развертывания
   - Сбор метрик и логов для анализа работы приложения
   - Обратная связь от команды разработки и операций для непрерывного улучшения пайплайна
7. Оптимизация и улучшение (Optimization and Improvement):
   - Анализ данных о прохождении пайплайна для выявления узких мест
   - Внедрение улучшений и оптимизаций для повышения производительности и качества поставки

Каждый из этих этапов играет важную роль в обеспечении непрерывной поставки изменений в продакшен и автоматизации процессов разработки.
#### Полный список практик DevOps:

1. Continuous Integration (непрерывная интеграция)
2. Continuous Delivery (непрерывная поставка)
3. Infrastructure as Code (инфраструктура как код)
4. Monitoring and Logging (мониторинг и логирование)
5. Collaboration and Communication (сотрудничество и коммуникация)
6. Automated Testing (автоматизированное тестирование)
7. Microservices (микросервисы)
8. Configuration Management (управление конфигурацией)
9. Containerization (контейнеризация)
10. Orchestration (оркестрация)
11. Version Control (управление версиями)
12. Deployment Automation (автоматизация развертывания)
13. Release Management (управление релизами)
14. Security Practices (практики безопасности)
15. Scalability and Elasticity (масштабируемость и эластичность)

Эти практики помогают компаниям создавать гибкие, надежные и высокопроизводительные системы, обеспечивая быструю поставку программного обеспечения и улучшение качества продукта.  
#### Что такое Continuous Integration/Delivery/Deployment и чем они друг от друга отличаются? 
(пример)  ![[cicd.png]]
#### CDl vs CDp
В случае Continuous Deployment каждый следующий шаг, будет выполнен автоматически если предыдущий был успешный, включая деплой на Production.

Если же у вас Continuous Delivery, то шаги будут выполняться автоматически только в безопасной среде, а перед деплоем на Production пайплайн остановится и будет ждать ручного подтверждения.  
  
Continuous deployment — осуществление доставки без какого-либо ручного воздействия и дополнительных подтверждений.

Continuous delivery — доставка «с кнопкой», здесь необходимо ручное вмешательство и сбор согласий.