### 1. Bases por Setor

- **Método**: `GET`
- **Endpoint**: `/api/bases-per-sector`
- **Descrição**: Retorna várias timelines de gráficos onde o eixo X representa o tempo e o eixo Y representa os valores.
- **Filtros**:
  - `sector` (opcional): Filtra por setor (ex.: indústria, serviços).
  - `variation` (opcional): Tipo de variação (ex.: real, dólar).
  - `timeFrame` (opcional): Período de tempo (ex.: mensal, anual, ou intervalo específico).
  
- **Resposta**:
  - **Status 200 (OK)**:
    ```json
    {
      "sector": "Indústria",
      "variation": "real",
      "data": [
        {
          "time": "2024-01-01",
          "value": 1500.50
        },
        {
          "time": "2024-02-01",
          "value": 1520.75
        }
      ]
    }
    ```

---

### 2. Bases por Cartão de Crédito

- **Método**: `GET`
- **Endpoint**: `/api/bases-x-credit-card`
- **Descrição**: Retorna várias timelines de gráficos com valores relacionados a bases de cartão de crédito.
- **Filtros**:
  - `sector` (opcional): Filtra por setor (ex.: tecnologia, saúde).
  - `variation` (opcional): Tipo de variação (real, dólar, etc.).
  - `timeFrame` (opcional): Período de tempo.
  
- **Resposta**:
  - **Status 200 (OK)**:
    ```json
    {
      "sector": "Serviços",
      "variation": "dólar",
      "data": [
        {
          "time": "2024-01-01",
          "value": 300.75
        },
        {
          "time": "2024-02-01",
          "value": 320.40
        }
      ]
    }
    ```

---

### 3. Emprego

- **Método**: `GET`
- **Endpoint**: `/api/employment`
- **Descrição**: Retorna várias timelines relacionadas ao emprego.
- **Filtros**:
  - `timeFrame` (opcional): Período de tempo.

- **Resposta**:
  - **Status 200 (OK)**:
    ```json
    {
      "data": [
        {
          "time": "2024-01-01",
          "employmentLevel": 5.2
        },
        {
          "time": "2024-02-01",
          "employmentLevel": 5.4
        }
      ]
    }
    ```

---

### 4. Salário vs Massa Salarial

- **Método**: `GET`
- **Endpoint**: `/api/salary-vs-mass-salary`
- **Descrição**: Retorna várias timelines de gráficos comparando salários com a massa salarial.
- **Filtros**:
  - `sector` (opcional): Filtra por setor.
  - `variation` (opcional): Tipo de variação (real, dólar, etc.).
  - `timeFrame` (opcional): Período de tempo.
  
- **Resposta**:
  - **Status 200 (OK)**:
    ```json
    {
      "sector": "Tecnologia",
      "variation": "real",
      "data": [
        {
          "time": "2024-01-01",
          "salary": 4500.50,
          "massSalary": 30000.00
        },
        {
          "time": "2024-02-01",
          "salary": 4600.00,
          "massSalary": 31000.00
        }
      ]
    }
    ```

---

### 5. Salário por Setor

- **Método**: `GET`
- **Endpoint**: `/api/sector-salary`
- **Descrição**: Retorna várias timelines de gráficos relacionados ao salário por setor.
- **Filtros**:
  - `sector` (opcional): Filtra por setor.
  - `timeFrame` (opcional): Período de tempo.
  
- **Resposta**:
  - **Status 200 (OK)**:
    ```json
    {
      "sector": "Agronegócio",
      "data": [
        {
          "time": "2024-01-01",
          "salary": 3000.00
        },
        {
          "time": "2024-02-01",
          "salary": 3100.00
        }
      ]
    }
    ```

---

### 6. Regional

- **Método**: `GET`
- **Endpoint**: `/api/regional`
- **Descrição**: Retorna várias timelines de gráficos por região.
- **Filtros**:
  - `sector` (opcional): Filtra por setor.
  - `UF` (opcional): Filtra por Unidade Federativa (ex.: SP, RJ).
  - `timeFrame` (opcional): Período de tempo.
  
- **Resposta**:
  - **Status 200 (OK)**:
    ```json
    {
      "region": "Sudeste",
      "UF": "SP",
      "data": [
        {
          "time": "2024-01-01",
          "value": 5000.00
        },
        {
          "time": "2024-02-01",
          "value": 5200.00
        }
      ]
    }
    ```
