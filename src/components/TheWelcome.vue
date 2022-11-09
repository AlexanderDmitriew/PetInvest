<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Зарегистрируйтесь на сайте</template>

    Простая форма
    <a href="#" target="_blank" rel="noopener">регистрации.</a>
    Нужна лишь ваша почта. Либо, войдите с помощью популярный социальных сетей.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Загрузите брокерский отчёт или подключите API Tinkoff</template>

    Ознакомьтесь с
    <a href="#" target="_blank" rel="noopener">Инструкцией для отчётов</a>.
    Или руководством по
    <a href="#" target="_blank" rel="noopener">Подключению Tinkoff API.</a>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Откройте аналитику</template>

    После подключения Вашего портфеля вы увидите:
    <a href="#" target="_blank" rel="noopener">Дивидендную доходность</a>,
    <a href="#" target="_blank" rel="noopener">Курсовую разницу цен</a>,
    <a href="#" target="_blank" rel="noopener">График изменения стоимости портфеля</a>, и
    <a href="#" target="_blank" rel="noopener">многое другое</a>. Наша система аналитики даёт большой объём информации о
    Вашем портфеле.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>Воспользуйтесь скринером</template>

    Если вы решите подобрать новые активы в свой портфель, то воспользуйтесь нашим
    <a href="#" target="_blank" rel="noopener">скринером</a> активов.
    По необходимым параметрам вы сможете найти подходящие бумаги.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Пользуйтесь бесплатно</template>

    Этот проект - просто проект без коммерческой основы. Если вы хотите поддержать, то перейдите по
    <a href="#" target="_blank" rel="noopener">ссылке</a>.
  </WelcomeItem>
</template>
